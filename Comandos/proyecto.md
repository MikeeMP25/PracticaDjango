### COMANDOS PARA UN NUEVO PROYECTO

Vamos a instalar los paquetes que vamos a utilizar para este proyecto.  
`pipenv install django django-ckeditor Pillow pylint pylint-django pylint-celery`  
**/framework/es un editor Wysiwing para editar campos/ gestionar imagenes/para mostrar los posibles errores de codigo de las importanciones**

Veficar donde sea instalado nuestro entorno virtual `pipenv --venv`

`pipenv run django-admin` podemos ver que tenemos diferentes comandos especificos de este script

Para crear un nuevo proyecto en django ejecutamos el siguiente comando.  
`pipenv run django-admin startproject webpersonal`  
imagen

Para poner en marcha el proyecto usamos el siguiente comando.
`python3 manage.py runserver` 
imagen captura.  

Para crear una nueva app dentro del proyecto utilizamos lo siguiente.   
`python3 manage.py startapp portfolio` 

