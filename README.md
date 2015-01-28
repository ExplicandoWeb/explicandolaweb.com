# Explicando La Web

Repositorio donde reside la base del sitio web de explicandolaweb.com
Montada sobre Django 1.7

# Requerimientos
* El fichero está alojado en la carpeta requirements
'pip install -r requirements.txt'


### Variables de entorno
Para mejorar la seguridad de las contraseñas se crearán las siguientes variables de entorno donde guardaremos las claves usadas
* KEY_DJANGO: Secret key de Django para el archivo de settings
* DB_NAME: con el nombre de la base de datos
* DB_USER: con el nombre de usuario de la base de datos
* DB_PASS: con el password de acceso a la base de datos


# Puesta en marcha
Una vez instalados los paquetes deberemos realizar la sincronización de la base de datos así como la aplicación de las migraciones. Esta sincronización dependerá del fichero de configuración que queramos usar.
- 'python manage.py syncdb --settings=exw.settings.dev'
- 'python manage.py migrate --settings=exw.settings.dev'
Arrancamos el proyecto con la siguiente instrucción
- 'python manage.py runserver --settings=exw.settings.dev'
