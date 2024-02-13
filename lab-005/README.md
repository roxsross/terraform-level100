**Detalles del Laboratorio:**

En este lab, estarás configurando una instancia EC2 y una instancia RDS, y luego establecer una conexión entre la instancia RDS y la instancia EC2 mediante Terraform.

**Requisitos Previos:**
1. Instala Terraform en tu máquina local siguiendo la guía oficial de Hashicorp.
   - Para instalar Terraform utilizando la CLI, consulta esta guía: [Instalación de Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli).
   - Para instalar Terraform descargándolo, sigue esta guía: [Descargas de Terraform](https://www.terraform.io/downloads).
2. Descarga e instala el editor Visual Studio Code siguiendo esta guía: [Descarga de Visual Studio Code](https://code.visualstudio.com/download).

**Detalles de la Tarea:**

0. **Diseña la Arquitectura**

1. **Crear un archivo de variables:**
   - Desarrolla un archivo de variables para gestionar los parámetros específicos del entorno.

2. **Crear un grupo de seguridad para RDS y EC2 en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar grupos de seguridad tanto para las instancias RDS como EC2.

3. **Agregar la instancia RDS en el archivo main.tf:**
   - Incluye configuraciones en el archivo `main.tf` para la creación de la instancia RDS.

4. **Agregar la creación de la instancia EC2 en el archivo main.tf:**
   - Amplía el archivo `main.tf` para incluir configuraciones de creación de la instancia EC2.

5. **Crear un archivo de salida:**
   - Desarrolla un archivo de salida para capturar información relevante generada durante la ejecución de Terraform.

6. **Aplicar las configuraciones de Terraform:**
   - Ejecuta los comandos de Terraform (`terraform init`, `terraform plan`, `terraform apply`) para aplicar las configuraciones y crear los recursos de las instancias EC2 y RDS.

7. **Verificar los recursos en la Consola de AWS:**
   - Accede a la Consola de AWS para confirmar la creación de recursos, especialmente las instancias EC2 y RDS.

8. **Crear una base de datos, tabla e insertar datos para pruebas:**
    - Establece una base de datos, crea una tabla e inserta datos con fines de prueba.
    ```
    CREATE DATABASE SchoolDB;
    show databases;
    use SchoolDB;
    CREATE TABLE IF NOT EXISTS subjects (subject_id INT AUTO_INCREMENT,subject_name VARCHAR(255) NOT NULL,teacher VARCHAR(255),start_date DATE,lesson TEXT,PRIMARY KEY (subject_id)) ENGINE=INNODB;
    show tables;
    INSERT INTO subjects(subject_name, teacher) VALUES ('English', 'John Taylor');
    INSERT INTO subjects(subject_name, teacher) VALUES ('Science', 'Mary Smith');
    INSERT INTO subjects(subject_name, teacher) VALUES ('Maths', 'Ted Miller');
    INSERT INTO subjects(subject_name, teacher) VALUES ('Arts', 'Suzan Carpenter');
    select * from subjects;
    exit;
``
9. **Validación del Laboratorio:**
    - Realiza las comprobaciones necesarias para asegurarte de que el entorno del laboratorio esté configurado y funcione según lo esperado.

10. **Eliminación de Recursos en AWS:**
    - Ejecuta el comando `terraform destroy` para eliminar los recursos de AWS creados durante el laboratorio.
