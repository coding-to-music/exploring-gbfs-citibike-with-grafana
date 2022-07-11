# exploring-gbfs-citibike-with-grafana

# 🚀 Visualizing metrics from the Node JS application with Prometheus and Grafana 🚀

https://github.com/coding-to-music/exploring-gbfs-citibike-with-grafana

From / By

Example of a Grafana dashboard, using data from Prometheus:

![Grafana screenshot](https://github.com/coding-to-music/exploring-gbfs-citibike-with-grafana/blob/main/images/example-dashboard.png?raw=true)

## Another good Grafana info source:

Grafana Dashboard with JSON APIs. visualize JSON, CSV, Graphql, XML in grafana

https://www.youtube.com/watch?v=Wmgs1E9Ry-s&ab_channel=SriramS

http://jsonviewer.stack.hu/

## Infinity Data source

https://github.com/yesoreyeram/grafana-infinity-datasource

https://sriramajeyam.com/grafana-infinity-datasource/

https://grafana.com/grafana/plugins/yesoreyeram-infinity-datasource/

## Citibike API

https://ride.citibikenyc.com/system-data

http://gbfs.citibikenyc.com/gbfs/gbfs.json

https://gbfs.citibikenyc.com/gbfs/en/station_status.json

## covid19api

https://api.covid19api.com

https://api.covid19api.com/summary

## Environment variables:

```java

```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/exploring-gbfs-citibike-with-grafana.git
git push -u origin main
```

## feed of feed topics from gbfs citibikenyc

http://gbfs.citibikenyc.com/gbfs/gbfs.json

```json
{
  "last_updated": 1657566300,
  "ttl": 5,
  "data": {
    "en": {
      "feeds": [
        {
          "name": "system_information",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/system_information.json"
        },
        {
          "name": "station_information",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/station_information.json"
        },
        {
          "name": "station_status",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/station_status.json"
        },
        {
          "name": "free_bike_status",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/free_bike_status.json"
        },
        {
          "name": "system_hours",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/system_hours.json"
        },
        {
          "name": "system_calendar",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/system_calendar.json"
        },
        {
          "name": "system_regions",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/system_regions.json"
        },
        {
          "name": "system_alerts",
          "url": "https://gbfs.citibikenyc.com/gbfs/en/system_alerts.json"
        }
      ]
    }
  }
}
```
