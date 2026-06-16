# NavigationApp Tiles

Static extracted Flight Maps tiles for NavigationApp.

Currently hosted layers:

- `CVFR`
- `Israel-Navigation`
- `LSA-Low-Altitude`
- `Israel-Helicopters`

URL pattern:

```text
https://navaid-tiles.supino.org/{layer}/{z}/{x}/{y}.png
```

Source MBTiles were downloaded from `https://flight-maps.com/` and extracted
to XYZ PNG tiles.
