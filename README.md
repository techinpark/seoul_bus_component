# Seoul Bus Component (HA)
🚎 Home Assistant (HA)  seoul bus arrival information custom component. 


# Usage 
- Setup your `sensor.yaml` 

## Options 
### Sensor options 
| Name | Type | Default | Since | Description |
|------|------|---------|-------|-------------|
| station_code | integer | **required** | v0.1 | bus stations code 
| name | string | **required** | v0.1 | stations name for display in dashboard.
| display | array | Optional | v0.1 | filter bus number for display arrival information
| hide | array | Optional | v0.1 | filter bus number for hide arrival information

```yaml
- platform: seoul_bus
  stations:
    - station_code: 12426
      name: 진관중고교
      show: 
        - 708
      hide: 
        - 7211
```
