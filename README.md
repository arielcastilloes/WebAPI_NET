# WebAPI_NET
Proyecto Tendencias Ing SW

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

