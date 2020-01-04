# Seoul Bus Component (HA)
🚎 Home Assistant (HA)  seoul bus arrival information custom component. 


# Usage 
- Setup your `sensor.yaml` 

## Options 
### Sensor options 
| Name | Type | Default | Since | Description |
|------|------|---------|-------|-------------|
| service_key | String | **required** | v0.1 | data api key (expired after 2year) 
| interval | integer | **required** | v0.1 | fetch interval for load api data 
| station_code | integer | **required** | v0.1 | bus stations code 
| name | string | **required** | v0.1 | stations name for display in dashboard.
| display | array | Optional | v0.1 | filter bus number for display arrival information
| hide | array | Optional | v0.1 | filter bus number for hide arrival information

```yaml
- platform: seoul_bus
  name: seoul_bus 
  service_key: [YOUR DATA API KEY HERE]
  interval: 180
  stations:
    - station_code: 12426
      name: 진관중고교
      show: 
        - 708
      hide: 
        - 7211
``` 
