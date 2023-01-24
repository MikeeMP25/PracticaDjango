### COMANDOS PARA MIGRAR LOS MODELOS A UNA BASE DE DATOS (SQLite)

nuestro proyeccto ya tiene plantillas precargadas y listas para usarse (tienes 14 migraciones sin aplicar para algunas apps)
`python3 manage.py migrate` esto nos servira para sincornizarnos con la base de datos y poder trabajar con ella.

__Nota: Debes de configurar la clase models.py de la app (portfolio)__

Crea el modelo de proyecto de migraciones: `python3 manage.py makemigrations portfolio` 

Aplica la migración a la base de datos: `python3 manage.py migrate portfolio` 

Comando para crear un super usuario "Administrador"  
`python3 manage.py createsuperuser`
   
Te pediran los siguientes datos:  
~~~
 - Username: "Mike"
 - e-mail: "jesus.libra619@gmail.com"
 - password: ******** 
~~~
