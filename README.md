

# User Manager

Ensure Docker is installed on your machine.

### Installation
* Clone the repository by entering the command `git clone https://github.com/kigold/UserManager.git` in the terminal.
* Navigate to the project folder using `cd UserManager` on your terminal (or command prompt)
* After cloning, run the application with the command `run.sh`, this command would set up container for the mongodb as well as the node app,
and also install all the dependencies for the node app, and then start the node app
* Open your browser and enter this url `http://localhost:3000/users` this list should be empty sine the database is blank
* Open Postman and create users using this url
    ```POST /users
    INPUT:

    name: John Doe
    email: john.doe@gmail.com
    password: johndoe```
* Add a couple of users as stated above, then revist `http://localhost:3000/users`, now you should find the users you just entered in the previous step.
For more indepth documentation on the API, check out
`https://github.com/BolajiOlajide/UserManager` from where i forked the node app.

### End Process
To stop the process at anytime, type this command in the termina `stop.sh`, this would stop all process and close the containers.
