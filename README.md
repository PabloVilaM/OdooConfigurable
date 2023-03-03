# Odoo

 - Primero tenemos que preparar el docker compose para subir el odoo y la base de datos. Este archivo se divide en 2 partes esencialmente.
 
  1. Primero tenemos la parte de la base de datos, en la cual especificamos nombre, contraseña, nombre de usuario, puertos y el nombre de la imagen.
  2. En la segunda parte del docker compose, tendriamos que especificar que depende de la bd para que no inicie sin ella, el nombre, el nombre del contenedor los puertos y lo mas importante, los volumenes, que nos servirán para acceder a los archivos de Odoo desde PyCharm.

 - Cuando ponemos los volumenes con los directorios correspondientes (en este caso, dentro del proyecto). Veremos que podermos interactuar con los archivos que componen el odoo desde PyCharm.

 - Por último, para enlazar la base de datos con el PyCharm, lo único que hay que hacer es ir a la derecha, darle a la pestaña de Database, darle al + y poner el usuario y las contraseñas especificadas en la segunda linea del README. Y ya estaria
