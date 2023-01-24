# COMANDOS DE PIPENV (ENTORNO VIRTUAL)

El primer requisito es contar con el intérprete de Python en el path del usuario.
- Consultar que version de python tienes instalada.  
`python3 --version`  a lo que nos referimos con python3 es llamar al ejecutable python3.exe    

- Vamos a instalar pipenv (el gestor de entornos virtuales)  
`pip3 install pipenv`

- Podemos consultar las opciones de Pipenv
`pipenv --help`  
- Para crear un entorno virtual y aqui le decimos que version queremos  
`pipenv --python 3.11`  
- Para saber en donde esta el directorio del entorno virtual que creamos usamos el sisguiente comando
`pipenv --venv` Esto significa que nosotros podemos utilizar el interprete del entorno virtual directamente  
- Para conseguir su ruta escribimos lo siguiente  
`pipenv --py`  
- Para lanzar el interprete de python del entorno virtual vamos a utilizar un comando `pipenv run python3` Estamos accediendo al python punto exe del interprete pero nuestro entorno virtual donde podemos hacer codigo directamente y salir con un exito ejecutando el método. 

Nota: Este python que hemos ejecutado es el del entorno virtual, no el de nuestro sistema.  


- Para ver que paquetes o librerias tengo instalados en el entorno virtual.  
`pipenv graph`  
- Para instalar cualquier paquete o lib en el entorno virtual.  
`pipenv install numpy`
Si recordaras lo que he dicho que tenemos tambien accesible el gestor de paquetes de Python3 (pip3) 

- Taambien podemos ejecutarlos con run si ponemos los siguiente (Para ver los paquetes que contiene mi entorno virtual).  
`pipenv run pip3 list`
Nota: Estamos haciendo lo mismo, pero aqui estamos utilizando el gestor de paquetes de python y aquí nos da un poco mas de información. 

- Vamos a acceder a la lista de todos los paquetes del Python del sistema operativo
- `pip list` 
  
Recordatorio esto es muy cómodo porque nos permite tener diferentes versiones de paquetes especificas para cada proyecto 


NOTA: Una vez creado el entorno virtual debes contemplar ciertas reglas de uso sobre un entorno vitual:  
  - No puedes renombrar el entorno virtual una vez creado.  
  - No puedes cambiar la ruta donde esta el directorio del entorno virtual.  

Para desinstalar un paquete del entorno virtual  
`pipenv uninstall numpy`
Para quitar el entorno virtual de proyecto  
`pipenv --rm`

OTRA FORMA DE EJECUTAR CIERTOS COMANDOS SON:  
- `pipenv run pip install numpay`  Para instalar un paquete.  
- `pipenv run pip list`  Para ver la lista de paquetes instalados.  
- `pipenv run pip uninstall numpy` Para desintalar un paquete   
  
 

Este comando es para inicializar el entorno virtual sobre el proyecto `pipenv shell` 
imagen captura

### COMANDOS PARA UN NUEVO PROYECTO

Para crear un nuevo proyecto en django ejecutamos el siguiente comando.  
`pipenv run django-admin startproject webpersonal`  

Para poner en marcha el proyecto usamos el siguiente comando.
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

