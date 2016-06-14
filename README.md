Pimatic Apple Location
=====================================

To use this app you need to install the Plugin "pimatic-apple-location".
You need to add a device to your Pimatic config for each Apple Device that should report it's location.

Plugin:

Simply add
```
    {
      "plugin": "apple-location"
    },
```
to your plugin configuration.

For each Device (Smartphone) you want to 'track', you need to create a corresponding device in your config.

If you want to use the Apple iCloud to locate your device your Device-Configuration should look like this:
```json
    {
      "id": "your-phone",
      "name": "your-phone",
      "class": "LocationDevice",
      "lat": 52.5200066,
      "long": 13.404954,
      "iCloudUser": "Username",
      "iCloudPass": "Password",
      "iCloudDevice": "DeviceName",
      "iCloudInterval": 60000
    },
```

The lat and long values correspond to the location you want the distance to be calculated.
You can use this website to get your longitude and latitude.
http://www.mapcoordinates.net/en
