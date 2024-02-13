**Detalles del Laboratorio:**
Este laboratorio te ayudará a mejorar la automatización y se enfoca en crear un sitio web estático alojado en un (bucket) de Amazon S3 utilizando Terraform.

**Introducción:**

*¿Qué es un Sitio Web Estático?*
Los sitios web estáticos representan la forma más elemental de presencia en línea y son notablemente sencillos de crear. En esencia, una página web estática se presenta al navegador web del usuario tal como está almacenada. Su contenido es fijo, cada página está codificada en HTML y ofrece la misma información a todos los visitantes. La creación de estos sitios no requiere habilidades avanzadas de programación web ni diseño de bases de datos. 

*¿Qué es Amazon S3?*
S3, cuyas siglas corresponden a Simple Storage Service, ofrece almacenamiento de objetos a través de una interfaz de servicio web. Cada objeto se guarda como un archivo con su metadato integrado y se le asigna un número de identificación único. Estos objetos se almacenan en contenedores llamados "Buckets", cuyos nombres son exclusivos globalmente y organizan el espacio de nombres de Amazon S3 en el nivel más alto. La creación de buckets por parte de Amazon S3 se ajusta a la región especificada y se pueden asignar permisos específicos para controlar el acceso y las transacciones de datos.

*¿Qué es Terraform?*
Terraform es una herramienta de software de Infraestructura como código (IaaC). Permite la definición y creación de recursos utilizando proveedores en un lenguaje de configuración declarativo. Terraform facilita el empaquetado y reutilización del código en forma de módulos, y ofrece soporte para diversos proveedores de infraestructura en la nube, como AWS, Azure, GCP, IBM Cloud, OCI, entre otros. Sus cuatro comandos principales son:
- `terraform init`
- `terraform plan`
- `terraform apply`
- `terraform destroy`

**Requisito previo:**
Instala Terraform en tu máquina local siguiendo la [guía oficial de Hashicorp](https://learn.hashicorp.com/tutorials/terraform/install-cli). Para instalar Terraform usando la CLI, utiliza [esta guía](https://learn.hashicorp.com/tutorials/terraform/install-cli). Para instalar Terraform descargándolo, utiliza [esta guía](https://www.terraform.io/downloads.html). Descarga e instala el editor Visual Studio Code utilizando [esta guía](https://code.visualstudio.com/download).

**Detalles del Lab:**

0. **Diseña la Arquitectura**

1. **Codigo Sitio Web :**
    - En la carpeta website se encuentra el código del sitio estatico
    ```
    .
├── assets
│   ├── favicon.ico
│   └── img
│       ├── avataaars.svg
│       └── portfolio
│           ├── cabin.png
│           ├── cake.png
│           ├── circus.png
│           ├── game.png
│           ├── safe.png
│           └── submarine.png
├── css
│   └── styles.css
├── index.html
└── js
    └── scripts.js
    ```

2. **Crear un archivo de variables:**
   - Crea un archivo de variables (puede llamarse, por ejemplo, `variables.tf`) para gestionar los parámetros específicos del entorno.

3. **Crear un Bucket de S3 y sus componentes en el archivo main.tf:**
   - Utiliza el archivo `main.tf` para definir y configurar el Bucket de S3 y sus componentes utilizando Terraform.

4. **Confirmar la instalación de Terraform:**
   - Verifica la instalación de Terraform asegurándote de que la versión esté correctamente configurada. Puedes hacer esto ejecutando el comando `terraform --version`.

5. **Aplicar la configuración de Terraform:**
   - Ejecuta los comandos de Terraform (`terraform init`, `terraform plan`, `terraform apply`) para aplicar la configuración y crear los recursos en AWS.

6. **Verificar los recursos en la Consola de AWS:**
   - Accede a la Consola de AWS para confirmar que los recursos (como el Bucket de S3) se hayan creado correctamente.

7. **Validación del laboratorio:**
   - Realiza las comprobaciones necesarias para asegurarte de que el entorno del laboratorio está configurado y funcionando según lo previsto.

8. **Eliminar recursos:**
   - Ejecuta el comando `terraform destroy` para eliminar los recursos creados y liberar los recursos en la nube.