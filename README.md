# MC game server


## [data folder](https://docker-minecraft-server.readthedocs.io/en/latest/data-directory/)

When attached in this way you can stop the server, edit the configuration under your attached directory and start the server again to pick up the new configuration.

```bash
sudo docker compose stop
# edit the configuration files under ./data
sudo docker compose start
```