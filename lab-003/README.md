**Detalles del Laboratorio:**

Este laboratorio te desafiará a través de la creación y prueba de una base de datos Amazon RDS MySQL utilizando Terraform.

**Requisitos Previos:**
1. Instala Terraform en tu máquina local siguiendo la guía oficial de Hashicorp.
   - Para instalar Terraform utilizando la CLI, consulta esta guía: [Instalación de Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli).
   - Para instalar Terraform descargándolo, sigue esta guía: [Descargas de Terraform](https://www.terraform.io/downloads).
2. Descarga e instala el editor Visual Studio Code siguiendo esta guía: [Descarga de Visual Studio Code](https://code.visualstudio.com/download).
3. Para probar este laboratorio, es necesario descargar la herramienta GUI de MySQL. Para hacerlo, ve a la página de descarga de MySQL Workbench. Según tu sistema operativo, selecciona la opción respectiva bajo "Generally Available (GA) Releases". Descarga e instala.

**Detalles de la Tarea:**

0. **Diseña la Arquitectura**

1. **Crear un archivo de variables:**
   - Crea un archivo de variables para gestionar los parámetros específicos del entorno.

2. **Crear un grupo de seguridad para la instancia RDS en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar un grupo de seguridad para la instancia RDS.

3. **Crear una instancia de base de datos RDS en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar la instancia de base de datos RDS.

4. **Crear un archivo de salida:**
   - Desarrolla un archivo de salida para capturar información relevante generada durante la ejecución de Terraform.

5. **Confirmar la instalación de Terraform verificando la versión:**
   - Asegúrate de que Terraform esté instalado correctamente verificando la versión. Ejecuta el comando `terraform --version`.

6. **Aplicar las configuraciones de Terraform:**
   - Ejecuta los comandos de Terraform (`terraform init`, `terraform plan`, `terraform apply`) para aplicar las configuraciones y crear los recursos de RDS.

7. **Verificar los recursos en la Consola de AWS:**
   - Accede a la Consola de AWS para confirmar la creación de recursos, especialmente la instancia de base de datos RDS.

8. **Probar la conexión a RDS utilizando MySQL Workbench:**
    - Utiliza MySQL Workbench para probar la conexión a la base de datos RDS.

9. **Validación del Laboratorio:**
    - Realiza las comprobaciones necesarias para asegurarte de que el entorno del laboratorio esté configurado y funcione según lo esperado.

10. **Eliminar los Recursos de AWS:**
    - Ejecuta el comando `terraform destroy` para eliminar los recursos de AWS creados durante el laboratorio.