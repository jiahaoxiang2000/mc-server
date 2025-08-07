# MC game server

## Features

### Thirst System
This server includes a simple thirst/drink system using the SimpleThirst plugin:

- **Thirst Bar**: Players have a thirst level (1-20) displayed in the action bar
- **Dehydration**: Thirst decreases over time, faster in hot biomes
- **Drinking**: Players can drink water bottles, milk, honey bottles to restore thirst
- **Environmental Effects**: 
  - Hot biomes (desert, badlands) increase thirst loss
  - Cold biomes (snowy areas) decrease thirst loss
- **Health Impact**: Low thirst causes damage over time

#### Drink Items:
- Water Bottle: +6 thirst
- Milk Bucket: +8 thirst  
- Honey Bottle: +4 thirst

#### Commands:
- `/thirst` - Check your current thirst level
- `/thirst reload` - Reload plugin config (admin only)

## [data folder](https://docker-minecraft-server.readthedocs.io/en/latest/data-directory/)

When attached in this way you can stop the server, edit the configuration under your attached directory and start the server again to pick up the new configuration.

```bash
sudo docker compose stop
# edit the configuration files under ./data
sudo docker compose start
```