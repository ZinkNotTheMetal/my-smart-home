# Initialization

When loading a new configuration Home Assistant will want to load it's own configuration first so here are the steps to get
our secrets and configuration.yml loaded

## In development mode

For anyone wanting to see the configuration work locally please ensure you have the prerequisites:

1. Docker
2. Location to put the files (I put mine on my mac /etc/docker/home-assistant)
3. If your location differs change .infrastructure/docker/docker-compose.yml

This script below

```sh
npm run dev
```

This will use the steps in the package.json to initialize a local instance of Home Assistant locally

## In Production mode

1. Install Home Assistant using the following [guide](https://www.home-assistant.io/installation/)
2. Run home assistant
3. Create distribution

   ```sh
   npm run dist
   ```

4. Deploy all configuration files
5. Deploy `secrets.yaml` file
6. Restart the server in the settings of Home Assistant
