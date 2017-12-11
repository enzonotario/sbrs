# SBRS
Se dispone de una imágen de Ubuntu 16.04 con todo lo necesario para utilizar **SBRS** con VirtualBox 5.2 [aquí](https://mega.nz/#!z1QB0JpS!2t3f2vijlHM_fYX_B0wHUX_UEvqUPMZiI0ydQ9zn9Dg)

- Descargar VirtualBox 5.2
    - [Windows](http://download.virtualbox.org/virtualbox/5.2.2/VirtualBox-5.2.2-119230-Win.exe)
    - [Otros](https://www.virtualbox.org/wiki/Download_Old_Builds_5_2)

Una vez descargada la imagen y VirtualBox, seguir los siguientes pasos:

- Descomprimir la imagen
- Abrir VirtualBox
- Hacer clic en "NUEVA" (en la parte superior)
- Seguir los pasos de instalación:
    - **Nombre y sistema operativo**
        - Nombre: Ubuntu-SBRS
        - Tipo: Linux
        - Versión: Ubuntu (64-bit)
    - **Tamaño de memoria**
        - Elegir el tamaño de memoria deseado (recomendado: 2GB)
    - **Disco duro**
        - Seleccionar ***Usar un archivo de disco duro virtual existente*** y seleccionar el archivo descargado *storage.vdi*

- Arrancar la máquina virtual

> Nota: La contraseña del usuario *root* es: **asdasd**

## Pasos para ejecutar SBRS
Abrir una terminal y ejecutar

`cd /home/enzo/SBRS && sh freeling.sh`

Abrir otra terminal y ejecutar

`cd /home/enzo/SBRS/sbrs-api && php artisan serve`

Abrir otra terminal y ejecutar

`sudo /home/enzo/solr-6.1.0/bin/solr start -e cloud -noprompt`

Abrir Firefox e ingresar a http://localhost/
