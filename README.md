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

This repository holds third-party mirrors only. Layers NavAid generates itself
(such as `CVFR-AIP`, built from the CAA's own CVFR sheets) live in
[`msupino/NavigationApp-owned-tiles`](https://github.com/msupino/NavigationApp-owned-tiles),
served from `https://msupino.github.io/NavigationApp-owned-tiles/{layer}/{z}/{x}/{y}.png`.
