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


## Steps

### Settings

1. Create a Github account if you don't have one.

2. Create a clean repository within the GitHub page with the name "Petstore-Challenge"

3. Create a folder on your computer called Petstore-Challenge and navigate to it in a console

4. Clone the following repository
    ``` shell
    git clone https://github.com/JuanManu59/Petstore.git
    ```
5. We go into the cloned repository folder and enter the command below to install Newman.
    ``` shell
    npm install -g newman
    ```
6. Newman is a command line Collection Runner for Postman. It allows you to run and test a Postman collection directly from the command line. It is designed with extensibility in mind so you can integrate it with your continuous integration servers and build systems.

7. Once Newman is installed, we proceed to enter the following command in the console:
    ``` shell
    newman run PetstoreCollection.postman_collection.json -e PetStoreEnvironment.postman_environment.json
    ```
8. Once this is done, you will see the results of the automated tests executed in the command console.

### End
