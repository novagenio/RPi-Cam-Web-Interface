# RPi-Cam-Web-Interface
RPi Cam Web Interface is a web interface for the Raspberry Pi Camera module. It can be used for a wide variety of applications including surveillance, dvr recording and time lapse photography. It is highly configurable and can be extended with the use of macro scripts. It can be opened on any browser (smartphones included) and contains the following features

Instalar RPI Cam Web

https://elinux.org/RPi-Cam-Web-Interface#Basic_Installation

La configuración de las opciones se encuentra en el fichero de configuración /etc/raspimjpeg, que es una imagen del original /RPi_Cam_Web_Interface/etc/raspimjpeg (que no sirve ojo). Leerlo es muy interesante.

Dentro de /etc/raspimjpeg, comentar la línea, #thumb_gen vit, si no queremos que genere los ficheros con el prefijo tm

# thumb generator control 
# Set v, i, or t in string to enable thumbs for images, videos, or lapse 
#thumb_gen vit      <-------------------------------- esta linea hay que comentara con un #
En el apartado #file location, se encuentra la definición y ubicación entre otras cosas, de las imágenes y las macros. Aquí ej. De las imágenes.

  image_path /var/www/html/media/im_%i_%Y%M%D_%h%m%s.jpg 
Y en el mismo /etc/raspimjpeg, la variable de entorno "rotation" para hacer que la camara rote 180 o n grados.
