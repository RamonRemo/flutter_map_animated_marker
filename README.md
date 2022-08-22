# flutter_map_animated_marker
Animated Marker for flutter_map

![preview](https://i.imgur.com/gRe67be.gif)


## Features

- Animated Marker

## Getting started

```yaml
dependencies:
    flutter_map_animated_marker:
```

## Usage

```dart
return FlutterMap(
      mapController: mapController,
      options: MapOptions(
          center: LatLng(51.509364, -0.128928),
          zoom: 9.2,
          plugins: [AnimatedMarkerPlugin()]),
      layers: [
        TileLayerOptions(
            urlTemplate: "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
          ),
        AnimatedMarkerLayerOptions(
            marker: Marker(
              point: LatLng(0, 0),
              builder: (context) => FlutterLogo(),
            ),
          ),
      ],
    );
```