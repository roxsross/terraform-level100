**Detalles del Laboratorio:**

En este laboratorio, estarás en el proceso de creación de una tabla DynamoDB e inserción de elementos en ella utilizando Terraform. 

**Requisitos Previos:**
1. Instala Terraform en tu máquina local siguiendo la guía oficial de Hashicorp.
   - Para instalar Terraform utilizando la CLI, consulta esta guía: [Instalación de Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli).
   - Para instalar Terraform descargándolo, sigue esta guía: [Descargas de Terraform](https://www.terraform.io/downloads).
2. Descarga e instala el editor Visual Studio Code siguiendo esta guía: [Descarga de Visual Studio Code](https://code.visualstudio.com/download).

**Detalles de la Tarea:**

0. **Diseña la Arquitectura**

1. **Crear un archivo de variables:**
   - Desarrolla un archivo de variables (por ejemplo, `variables.tf`) para gestionar parámetros específicos del entorno.

2. **Crear una Tabla DynamoDB y sus componentes en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar la Tabla DynamoDB y sus componentes mediante Terraform.

3. **Agregar elementos a la Tabla DynamoDB:**
   - Implementa la adición de elementos a la Tabla DynamoDB mediante Terraform.
   ```
        {
        "id": {"S": "something"},
        "one": {"N": "11111"},
        "two": {"N": "22222"},
        "three": {"N": "33333"},
        "four": {"N": "44444"}
        }
   ```
4. **Crear un archivo de salida:**
   - Desarrolla un archivo de salida para capturar información relevante generada durante la ejecución de Terraform.

5. **Confirmar la instalación de Terraform verificando la versión:**
   - Asegúrate de que Terraform esté instalado correctamente verificando la versión. Ejecuta el comando `terraform --version`.

6. **Aplicar las configuraciones de Terraform:**
   - Ejecuta los comandos de Terraform (`terraform init`, `terraform plan`, `terraform apply`) para aplicar las configuraciones y crear los recursos de DynamoDB.

7. **Verificar los recursos en la Consola de AWS:**
   - Accede a la Consola de AWS para confirmar la creación de recursos, especialmente la Tabla DynamoDB.

8. **Eliminación de Recursos en AWS:**
    - Ejecuta el comando `terraform destroy` para eliminar los recursos de AWS creados durante el laboratorio.