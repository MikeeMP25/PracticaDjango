# COMANDOS DE PIPENV (ENTORNO VIRTUAL)

- Consultar que version de python tienes instalada  
`python3 --version`  

- Instalar pipenv (El entorno virtual)  
`pip3 install pipenv`

- Verificar que este instalado correctamente  
`pipenv --help`  
- Crear un entorno virtual  
`pipenv --python 3.11`  
- Para saber en donde esta el directorio del entorno virtual que creamos 
`pipenv --venv` o podemos usar el interprete de python directamente para saber la ruta `pipenv --py`
- Para entrar a un archivo .py de forma normal pero en virtual.  
`pipenv run python3`    
- Para ver que paquetes o librerias tengo instalados en el entorno virtual.  
`pipenv graph`
- Para instalar cualquier paquete o lib en el entorno virtual.  
`pipenv install numpy`
- Para ver los paquetes que contiene mi entorno virtual.  
`pipenv run pip3 list`

NOTA: Una vez creado el entorno virtual debes contemplar ciertas reglas de uso sobre un entorno vitual:  
  - No puedes renombrar el entorno virtual una vez creado.  
  - No puedes cambiar la ruta donde esta el directorio del entorno virtual.  

- Para desinstalar un paquete del entorno virtual
   `pipenv uninstall numpy`
   
OTRA FORMA DE EJECUTAR CIERTOS COMANDOS SON:  
- `pipenv run pip install numpay`  Para instalar un paquete.  
- `pipenv run pip list`  Para ver la lista de paquetes instalados.  
- `pipenv run pip uninstall numpy` Para desintalar un paquete     
  
Para quitar el entorno virtual de proyecto `pipenv --rm` 

Este comando es para inicializar el entorno virtual sobre el proyecto `pipenv shell` 
imagen captura

### COMANDOS PARA UN NUEVO PROYECTO

Para crear un nuevo proyecto en django ejecutamos el siguiente comando.  
`pipenv run django-admin startproject webpersonal`  

Para ejecutar el proyecto con Django usamos el siguiente comando.
`python3 manage.py runserver` 
imagen captura.  

Para crear una nueva app dentro del proyecto utilizamos lo siguiente.   
`python3 manage.py startapp portfolio` 


### COMANDOS PARA MIGRAR LOS MODELOS A UNA BASE DE DATOS (SQLite)

__Nota: Debes de configurar la clase models.py de la app (portfolio)__

Crea el modelo de proyecto de migraciones: `python3 manage.py makemigrations portfolio`  
Aplica la migración a la base de datos: `python3 manage.py migrate portfolio` 

Comando para crear un super usuario "Administrador" `python3 manage.py createsuperuser`
   
Te pediran los siguientes datos:  
~~~
 - Username: "Mike"
 - e-mail: "jesus.libra619@gmail.com"
 - password: ******** 
~~~





  
