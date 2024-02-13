**Detalles del Laboratorio:**

Este laboratorio te permite prácticar conceptos y crear una Virtual Private Cloud (VPC) de dos niveles utilizando Terraform.

**Introducción:**

**¿Qué es una VPC?**
VPC significa Virtual Private Cloud.

Es una red virtual personalizada dentro de la Nube de AWS.

Los usuarios pueden crear lógicamente su propia red, diseñando e implementando una red separada e independiente que operaría en la Nube de AWS.

Los componentes principales incluyen Subredes, Direcciones IP, Dispositivos NAT (Instancias y Puertas de Enlace), Tablas de Rutas, Puertas de Enlace de Internet y Virtuales Privadas, Listas de Control de Acceso, Grupos de Seguridad, Puntos de Enlace de VPC.

Una subred es un segmento del rango de direcciones IP de la VPC, donde podemos lanzar instancias EC2, RDS y otros recursos de AWS.

Las subredes se clasifican como Públicas y Privadas.

**Entendimientos Básicos antes de comenzar a construir la VPC desde cero:**
Cuando creas una VPC de Amazon AWS, especificas un conjunto de direcciones IP en forma de bloque CIDR (por ejemplo, 10.0.0.0/16).

Puedes asignar un solo bloque CIDR a una VPC. El tamaño del bloque permitido va desde una máscara de red /28 hasta una máscara de red /16. En otras palabras, la VPC puede contener desde 16 hasta 65,536 direcciones IP.

**Requisito Previo:**
Instala Terraform en tu máquina local siguiendo la guía oficial de Hashicorp.
- Para instalar Terraform utilizando la CLI, consulta esta guía: [Instalación de Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli).
- Para instalar Terraform descargándolo, sigue esta guía: [Descargas de Terraform](https://www.terraform.io/downloads).
Descarga e instala el editor Visual Studio Code siguiendo esta guía: [Descarga de Visual Studio Code](https://code.visualstudio.com/download).

**Detalles de la Tarea:**

0. **Diseña la Arquitectura**

1. **Crear un archivo de variables:**
   - Crea un archivo de variables para gestionar los parámetros específicos del entorno.

2. **Crear VPC y sus componentes en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar la VPC y sus componentes mediante Terraform.

3. **Confirmar la instalación de Terraform verificando la versión:**
   - Asegúrate de que Terraform esté instalado correctamente verificando la versión. Ejecuta el comando `terraform --version`.

4. **Aplicar las configuraciones de Terraform:**
   - Ejecuta los comandos de Terraform (`terraform init`, `terraform plan`, `terraform apply`) para aplicar las configuraciones y crear los recursos de la VPC.

5. **Verificar los recursos en la Consola de AWS:**
   - Accede a la Consola de AWS para confirmar la creación de recursos, especialmente la VPC y sus componentes.

6. **Validación del Laboratorio:**
   - Realiza las comprobaciones necesarias para asegurarte de que el entorno del laboratorio esté configurado y funcione según lo esperado.