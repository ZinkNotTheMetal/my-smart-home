# Getting Started w/ my Smart home Configuration

## Services Utilized

- [Home Assistant](https://www.home-assistant.io)
- [Node-Red](https://nodered.org)
- [MQTT](https://mqtt.org)

## Home Assistant

Home Assistant is the workhorse of the smart home. It is where all of the integrations into third party services / sensors live. This is where I configure any integrations such as Philips Hue, SONOS, or the current wind speed.

## Node Red

Node Red is the automation work horse it has a great UI and an intuitive flow that makes it super simple to get started drawing and laying out automations. I also like the fact that I can test an automation super simply by adding the timestamp start point and click and test out that things work. I recommend this if the Home Assistant automations seem cumbersome or not intuitive.

## MQTT

MQTT is a lightweight and efficient message broker. It is really designed for the Internet of Things (IoT) space and is used in many setups. It supports a wide variety of integrations and a good tool to have and know. The best analogy I heard for this is it's like a whiteboard in an office. Not everyone can get into the office, not everyone cares about what is written on it, but the certain few that do it's a great place to write and update the team on what's happening.

## Development Mode

How can I get your configuration up and running to see if I like it?

Some prerequisites are needed:

- Test Machine w/ Docker Desktop installed
- NPM installed (not that necessary but just made it easier)
- File storage (you will need a folder to install the git repo and files needed)

### Running the docker-compose

 1. If it's your first time running this configuration read the first time steps below

 2. Run script below to run all services

    ```sh
    npm run dev
    ```

## Production Mode

 1. If it's your first time running this configuration read the first time steps below

 2. Ensure that your .env file is named .env.prod

 3. Run script below to run all services

    ```sh
    npm run start
    ```

## First time steps

 1. Copy the .env.example to a test one

    ```sh
    cp <git_directory>/my-smart-home/.infrastructure/docker/.env.example .env
    ```

 2. Fill out environment variables to your liking

 3. Copy the secrets.example.yaml to the base home-assistant directory

    ```sh
    cp <git_directory>/my-smart-home/secrets.example.yaml <git_directory>/src/home-assistant/secrets.yaml
    ```
  
 4. Fill in secrets in the new home-assistant directory

 5. Copy the mosquitto example config into the <docker_directory>/mqtt/config

    ```sh
    cp <git_directory>/.infrastructure/mqtt/mosquitto.conf.example mosquitto.conf
    ```

 6. Comment out the Authentication at first
 7. Run the command to setup a new user

    ```sh
    docker exec -it mqtt mosquitto_passwd -c /mosquitto/config/mqttuser hauser
    ```

 8. Choose a password for this user (it will be encrypted and hashed)

 9. You're done, go back to the run steps above
