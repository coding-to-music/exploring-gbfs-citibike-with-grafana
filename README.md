# exploring-gbfs-citibike-with-grafana

# 🚀 Visualizing metrics from the GBFS feed from citibikenyc with Grafana 🚀

https://github.com/coding-to-music/exploring-gbfs-citibike-with-grafana

From / By

See also:

https://github.com/coding-to-music/mongodb-iot-reference-citibike-cron-jobs

https://github.com/coding-to-music/mongodb-iot-reference-citibike-cron-jobs/blob/main/mongodb-timeseries/README.md

Citi Bike publishes real-time system data in GBFS General Bikeshare Feed Specification format. https://github.com/NABSA/gbfs/blob/master/gbfs.md

Get the GBFS feed here: http://gbfs.citibikenyc.com/gbfs/gbfs.json

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

## System Data

Where do Citi Bikers ride? When do they ride? How far do they go? Which stations are most popular? What days of the week are most rides taken on? We've heard all of these questions and more from you, and we're happy to provide the data to help you discover the answers to these questions and more. We invite developers, engineers, statisticians, artists, academics and other interested members of the public to use the data we provide for analysis, development, visualization and whatever else moves you.

This data is provided according to the Citi Bike Data Use Policy.

## Citi Bike Trip Histories

We publish downloadable files of Citi Bike trip data. https://s3.amazonaws.com/tripdata/index.html

The data includes:

- Ride ID
- Rideable type
- Started at
- Ended at
- Start station name
- Start station ID
- End station name
- End station ID
- Start latitude
- Start longitude
- End latitude
- End Longitude
- Member or casual ride

Data format previously:

- Trip Duration (seconds)
- Start Time and Date
- Stop Time and Date
- Start Station Name
- End Station Name
- Station ID
- Station Lat/Long
- Bike ID
- User Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
- Gender (Zero=unknown; 1=male; 2=female)
- Year of Birth

This data has been processed to remove trips that are taken by staff as they service and inspect the system, trips that are taken to/from any of our “test” stations (which we were using more in June and July 2013), and any trips that were below 60 seconds in length (potentially false starts or users trying to re-dock a bike to ensure it's secure).

Please be aware of your software program’s row limitations as you are viewing the data. Many of the CSV files contain more than 1 million rows. After downloading, you will need to use a large data tool / visualizer (like Tableau, Alteryx, R, or others) to view and analyze the full data sets.

Download Citi Bike trip history data: https://s3.amazonaws.com/tripdata/index.html

## Real-Time Data

Citi Bike publishes real-time system data in General Bikeshare Feed Specification format. https://github.com/NABSA/gbfs/blob/master/gbfs.md

Get the GBFS feed here: http://gbfs.citibikenyc.com/gbfs/gbfs.json

## Monthly Operating Reports

View the monthly operating reports that we provide to the NYC Department of Transportation.

https://ride.citibikenyc.com/system-data/operating-reports

## Additional Resources

- The City of New York's bicycling data http://www.nyc.gov/html/dot/html/about/datafeeds.shtml#Bikes
- A group of software developers and data explorers working with data feeds from NYC's Bike Share system and other bike data maintain this Google Group (note: Citi Bike is not responsible for this group – it is run and maintained by a group of interested private citizens) https://groups.google.com/forum/#!aboutgroup/citibike-hackers

## Community articles and helpful info

By Clif Kranish https://medium.com/@ckranish

Explorer of data and bicycle routes. Leader in agile product management for data access and data preparation.

https://towardsdatascience.com/estimating-bike-availability-from-nyc-bike-share-data-7cfc4655d5f6

https://towardsdatascience.com/interpolating-nyc-bike-share-data-to-discover-rebalancing-movements-6cf8a80eb902

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

## system_information

```
{
  "name": "station_information",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/system_information.json"
},
```

```json
{
  "data": {
    "system_id": "NYC",
    "email": "customerservice@motivateco.com",
    "name": "Citi Bike",
    "license_url": "",
    "phone_number": "1-855-BIKE-311",
    "language": "en",
    "operator": "Motivate International, Inc.",
    "url": "http://www.citibikenyc.com",
    "purchase_url": "http://www.citibikenyc.com/",
    "start_date": "2013-05-01",
    "timezone": "America/New_York",
    "short_name": "Citi Bike"
  },
  "last_updated": 1657569155,
  "ttl": 5
}
```

## station_information

```
{
  "name": "station_information",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/station_information.json"
},
```

```json
{
  "data": {
    "stations": [
      {
        "lon": -73.99392888,
        "rental_uris": {
          "android": "https://bkn.lft.to/lastmile_qr_scan",
          "ios": "https://bkn.lft.to/lastmile_qr_scan"
        },
        "station_id": "72",
        "name": "W 52 St & 11 Ave",
        "eightd_station_services": [],
        "external_id": "66db237e-0aca-11e7-82f6-3863bb44ef7c",
        "eightd_has_key_dispenser": false,
        "has_kiosk": true,
        "legacy_id": "72",
        "capacity": 55,
        "rental_methods": ["CREDITCARD", "KEY"],
        "region_id": "71",
        "lat": 40.76727216,
        "station_type": "classic",
        "electric_bike_surcharge_waiver": false,
        "short_name": "6926.01"
      },
      {
        "lon": -74.00666661,
        "rental_uris": {
          "android": "https://bkn.lft.to/lastmile_qr_scan",
          "ios": "https://bkn.lft.to/lastmile_qr_scan"
        },
        "station_id": "79",
        "name": "Franklin St & W Broadway",
        "eightd_station_services": [],
        "external_id": "66db269c-0aca-11e7-82f6-3863bb44ef7c",
        "eightd_has_key_dispenser": false,
        "has_kiosk": true,
        "legacy_id": "79",
        "capacity": 33,
        "rental_methods": ["CREDITCARD", "KEY"],
        "region_id": "71",
        "lat": 40.71911552,
        "station_type": "classic",
        "electric_bike_surcharge_waiver": false,
        "short_name": "5430.08"
      }
    ]
  }
}
```

## station_status

```json
{
  "name": "station_status",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/station_status.json"
},
```

```json
{
  "data": {
    "stations": [
      {
        "is_renting": 0,
        "last_reported": 1656077952,
        "is_returning": 0,
        "is_installed": 0,
        "num_bikes_available": 0,
        "legacy_id": "72",
        "num_docks_available": 55,
        "num_docks_disabled": 0,
        "station_status": "out_of_service",
        "num_bikes_disabled": 0,
        "num_ebikes_available": 0,
        "eightd_has_available_keys": false,
        "station_id": "72"
      },
      {
        "is_renting": 1,
        "last_reported": 1657569936,
        "is_returning": 1,
        "is_installed": 1,
        "num_bikes_available": 30,
        "legacy_id": "79",
        "num_docks_available": 2,
        "num_docks_disabled": 0,
        "station_status": "active",
        "num_bikes_disabled": 0,
        "num_ebikes_available": 4,
        "eightd_has_available_keys": false,
        "station_id": "79"
      },
      {
        "is_renting": 1,
        "last_reported": 1657570099,
        "is_returning": 1,
        "is_installed": 1,
        "num_bikes_available": 26,
        "legacy_id": "82",
        "num_docks_available": 1,
        "num_docks_disabled": 0,
        "station_status": "active",
        "num_bikes_disabled": 0,
        "num_ebikes_available": 0,
        "eightd_has_available_keys": false,
        "station_id": "82"
      }
    ]
  }
}
```

## free_bike_status

```json
{
  "name": "free_bike_status",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/free_bike_status.json"
},
```

```json
{
  "data": {
    "bikes": []
  },
  "last_updated": 1657570230,
  "ttl": 5
}
```

## system_hours

```json
{
  "name": "system_hours",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/system_hours.json"
},
```

```json
{
  "data": {
    "rental_hours": []
  },
  "last_updated": 1657570160,
  "ttl": 5
}
```

## system_calendar

```json
{
  "name": "system_calendar",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/system_calendar.json"
},
```

```json
{
  "data": {
    "calendars": [
      {
        "end_day": 31,
        "start_month": 1,
        "start_day": 1,
        "end_month": 12
      }
    ]
  },
  "last_updated": 1657570115,
  "ttl": 5
}
```

## system_regions

```json
{
  "name": "system_regions",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/system_regions.json"
},
```

```json
{
  "data": {
    "regions": [
      {
        "region_id": "70",
        "name": "JC District"
      },
      {
        "region_id": "71",
        "name": "NYC District"
      },
      {
        "region_id": "158",
        "name": "8D"
      },
      {
        "region_id": "185",
        "name": "Bronx"
      },
      {
        "region_id": "189",
        "name": "IC HQ"
      },
      {
        "region_id": "190",
        "name": "testzone"
      },
      {
        "region_id": "311",
        "name": "Hoboken District"
      }
    ]
  },
  "last_updated": 1657570060,
  "ttl": 5
}
```

## system_alerts

```json
{
  "name": "system_alerts",
  "url": "https://gbfs.citibikenyc.com/gbfs/en/system_alerts.json"
}
```

```json
{
  "data": {
    "alerts": [
      {
        "times": [
          {
            "end": 1584590340,
            "start": 1582084680
          }
        ],
        "last_updated": 1582136654,
        "alert_id": "101",
        "description": "Annual Members ride for only $0.10 per minute",
        "summary": "Ride further with our new ebikes",
        "type": "OTHER",
        "url": "https://www.citibikenyc.com/how-it-works/electric"
      }
  }
  "last_updated": 1657569900,
  "ttl": 5
}
```
