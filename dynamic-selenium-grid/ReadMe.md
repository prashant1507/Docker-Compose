##  _Dynamic Grid_

1. Docker demon should be accessible. Temporary below command can be executed
   ```
    sudo socat tcp-listen:2375,reuseaddr,fork,bind=192.168.0.142 unix-client:/var/run/docker.sock,su=root
   ```
2. Set IP:PORT in [config.toml](config.toml)
3. Set config.toml in [docker-compose-dynamic-grid.yml](docker-compose-dynamic-grid.yml)
4. Run `docker-compose up`

### Notes:
- Currently, the compose file and config.toml os not supporting video recording
- Command in step 1 is just a workaround.
