# Drone CI

## To Use:

Follow the directions at:

- https://docs.drone.io/server/provider/github/
- https://docs.drone.io/runner/docker/installation/linux/

The environment variables can be filled in via the .env files. For a template, you can copy the `.example.env*` files and naming the copies by removing the `.example` portion from the front and filling in the values.

Once the values are filled in for your environment, run:
`docker-compose up -d` and the drone server and runner should start.

### Note:

You will need to port-forward port 80 to the host your drone container is running on in order to receive webhooks from github for automated builds.
