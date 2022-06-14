## Petstore Challenge

Using the following API Definition: https://petstore.swagger.io/#/
Create a collection with two requests:
1. Create a Pet, create tests to verify it was created successfully
2. Get a Pet, create tests to verify you're getting the expected pet
3. Place an order for the created Pet
4. Get the order created in step 3, and verify it has the expected data.
5. Automate it using newman

Hint: You will probably need to use environments to store some data that needs to be shared between requests.

Upload the solution to a repo, put in the README instructions about how to execute your code, share the solution as a response to this message :)


##Steps

###1. Configuración inicial

1. Crear una cuenta en Github si no la tiene.

2. Crear un repositorio en limpio dentro de la página de GitHub con el nombre de “Petstore-Challenge”

3. Crear una carpeta en su computador llamada Petstore-Challenge y ubicarse en ella en una consola

4. Clonar el siguiente repositorio

    ``` shell
    git clone https://github.com/JuanManu59/Petstore.git
    ```
5. Ingresamos a la carpeta del repositorio clonado e ingresamos el comando a continuación para instalar Newman.
    ``` shell
    npm install -g newman
    ```
6. Newman es un Collection Runner de línea de comandos para Postman. Le permite ejecutar y probar una colección de Postman directamente desde la línea de comandos. Está diseñado pensando en la extensibilidad para que pueda integrarlo con sus servidores de integración continua y sistemas de compilación.

7. Una vez instalado Newman procedemos a ingresar el siguiente comando en la consola:
    ``` shell
    newman run PetstoreCollection.postman_collection.json -e PetStoreEnvironment.postman_environment.json
    ```
8. Una vez hecho esto verá en la consola de comandos los resultados de las pruebas automatiadas ejecutadas.

###End