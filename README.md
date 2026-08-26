# NavigationApp Tiles

Static extracted Flight Maps tiles for NavigationApp.

Currently hosted layers:

- `CVFR`
- `CVFR-AIP`
- `Israel-Navigation`
- `LSA-Low-Altitude`
- `Israel-Helicopters`

URL pattern:

```text
https://navaid-tiles.supino.org/{layer}/{z}/{x}/{y}.png
```

Source MBTiles were downloaded from `https://flight-maps.com/` and extracted
to XYZ PNG tiles.

`CVFR-AIP` is built here rather than downloaded. Its source is the CAA's own
two CVFR sheets (AIP part II, northern and southern), which are vector PDFs, so
the tiles carry the track bearings, leg distances and altitude flags the
extracted Flight Maps set does not. z8-13, 3,768 tiles. Built with
`scripts/build-cvfr-tiles.py` in the NavigationApp repo:

```text
python3 scripts/build-cvfr-tiles.py cvfr-north.pdf cvfr-south.pdf --out CVFR-AIP
```
