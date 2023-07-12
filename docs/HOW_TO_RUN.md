## Development Mode

Q?: How can I get your configuration up and running to see if I like it?

Some prerequisites are needed:

*   Computer w/ Docker Desktop installed (Linux, Mac, or Windows)
*   NPM installed (not that necessary but just makes some things easier)
*   File storage (you will need a folder to install the git repo and files needed)

### Running the docker-compose

1.  If it's your first time running this configuration read the first time steps below
2.  Run script below to run all services

    ```sh
    npm run dev
    ```

## Production Mode

1.  If it's your first time running this configuration read the first time steps below
2.  Ensure that your .env file is named .env.prod
3.  Run script below to run all services

    ```sh
    npm run start
    ```

## First time steps

1.  Copy the .env.example to a test one

    ```sh
    cp <git_directory>/my-smart-home/.infrastructure/docker/.env.example .env
    ```

2.  Fill out environment variables to your liking

3.  Copy the secrets.example.yaml to the base home-assistant directory

    ```sh
    cp <git_directory>/my-smart-home/secrets.example.yaml <git_directory>/src/home-assistant/secrets.yaml
    ```

4.  Fill in secrets in the new home-assistant directory

5.  Copy the mosquitto example config into the \<docker\_directory>/mqtt/config

    ```sh
    cp <git_directory>/.infrastructure/mqtt/mosquitto.conf.example mosquitto.conf
    ```

6.  Comment out the Authentication at first

7.  Run the command to setup a new user

    ```sh
    docker exec -it mqtt mosquitto_passwd -c /mosquitto/config/mqttuser hauser
    ```

8.  Choose a password for this user (it will be encrypted and hashed)

9.  You're done, go back to the run steps above
