# WEB API EN .NET PARA GESTION DE LIBROS CON API SWAGGER


<b>Proyecto Tendencias Ing SW </b>

El siguiente ejercicio corresponde con una aplicación construida en C# para la administración de API y creación de Libros y sus relaciones de autor con Swagger. Adicionalmente se tiene una conexión a una BD SQL que se instalarán en dos contenedores de Docker

<b> 1. ESTRUCTURA DEL PROYECTO </b>

En la siguiente pantalla se puede ver los componentes más relevantes que hacen parte del proyecto que se describen y se describen continuación:

![image](https://user-images.githubusercontent.com/104280126/173203641-fcd0c242-53a4-4dd1-8538-402803543e11.png)

Controllers/V1: En este apartado se encuentra todo el domino de negocio del proyecto para la implementación de la solución de las API y manejo de lógica para poder persistr en la BD correspondiente.

DTO: Estructura de datos para el proyecto donde se encuentran las definiciones de la información que vamos a gestionar.

Models/PreparDB: Clase para gestionar y configurar parámetros para establecer conexión de BD.

Dockerfile, .dockerignore y docker-compose.yaml : Estos archivos de configuración nos permitirán orquestar los servicios para poder desplega en Docker.

<b> 2. CONFIGURACIÓN </b>

<b> Dokerfile: </b>

![image](https://user-images.githubusercontent.com/104280126/173204225-3b5d5d7a-943d-45fc-a687-894d85045953.png)

<b> .dockerignore: </b>

![image](https://user-images.githubusercontent.com/104280126/173204264-e0761e49-fff1-4667-a2ab-09a176d98df0.png)


<b> docker-compose.yaml: </b>

![image](https://user-images.githubusercontent.com/104280126/173204277-5d1e1cb8-3e54-4acd-bee9-d6a4e9a97125.png)


<b> 3. DEPLOY DOCKER </b>

Se procede a ejecutar los siguientes comandos para construir y ejecutar la orquestación :


<b> docker-compose build </b> 

![image](https://user-images.githubusercontent.com/104280126/173204674-0e3e7787-1e7b-4456-a234-026ae74d7fad.png)


<b> docker-compose up </b>

![image](https://user-images.githubusercontent.com/104280126/173204686-026c1a85-92b9-4dea-9c3e-ebb221a01009.png)


Se hace la validación en nuestro Docker para Windows y se validan que se hayan montado las imágenes:

![image](https://user-images.githubusercontent.com/104280126/173204751-7ce3a67f-8615-497c-aca5-15f1ca1d70a5.png)


Los contenedores / apps:

![image](https://user-images.githubusercontent.com/104280126/173204767-cb491f4c-6243-4e69-90fb-99adf2f9eb9d.png)


Ahora validamos que se haya desplegado nuestra aplicación y nuestra BD. 

![image](https://user-images.githubusercontent.com/104280126/173204793-00c30145-590f-4095-b4dd-3a67b6fdb1fd.png)

La conexión a la BD se hace con un cliente de BD DBeaver:

![image](https://user-images.githubusercontent.com/104280126/173204813-35f8ddcf-2827-4739-87bb-43b3c43ef301.png)


Se hace la prueba creando un usuario desde la APP y validando contra la BD:

![image](https://user-images.githubusercontent.com/104280126/173204885-a99433fb-b73b-42d2-bba4-3f0516b82f70.png)
![image](https://user-images.githubusercontent.com/104280126/173204893-05883427-7fff-4f0d-b4a0-56e5464d0735.png)


Se realiza la consulta en la BD para evidenciar la creación en la tabla autores:

![image](https://user-images.githubusercontent.com/104280126/173204917-a84f225f-8fc3-45a7-9053-1a6333785e6d.png)



