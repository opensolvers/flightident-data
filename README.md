# Flightident data

Static files the Flightident app reads. This repository does not replace GoDrone or a NOTAM.

Sources, download dates and licences are kept in [BRONNEN.md](BRONNEN.md).

## Netherlands

`nl/uas-zones.json` is the UAS geographical zone set for the Amsterdam FIR, in EUROCAE ED-269 JSON.

- Source: the direct download named in AIP Netherlands, ENR 5.3
- File: `Alle statische zonering en andere gebieden in ED269 format - 22juli2024.JSON`
- Issued: 22 July 2024
- Contents: 774 zones (10 prohibited, 51 requiring authorisation, 713 conditional)

The AIP requires this information to be publicly available under Article 15 of Regulation (EU) 2019/947. The copy here is unchanged from that download.

### Areas

`nl/gebieden/` splits those 774 zones into GeoJSON files. Circles from the ED-269 file are drawn as 64-point polygons. `nl/gebieden/index.json` lists the files and the rule text from the source.

| File | Areas | What it contains |
| --- | --- | --- |
| `verboden.geojson` | 10 | Closed to all flights, including the 4 May memorials |
| `beveiligd.geojson` | 338 | Secured sites and vital processes; open category forbidden |
| `industrie.geojson` | 270 | Major-accident industrial sites, including Westpoort |
| `vliegvelden.geojson` | 43 | Aerodrome proximity, including CTRs |
| `defensie.geojson` | 67 | Military areas; open category forbidden, several only with military ATC permission |
| `helikopter.geojson` | 23 | Trauma and rescue helicopter landing sites |
| `laagvlieg.geojson` | 23 | Low-flying and helicopter firefighting areas; A1/A2 up to 30 m, A3 not allowed |

`natura2000.geojson` is separate. It holds 209 Natura 2000 boundaries from PDOK (Rijksdienst voor Ondernemend Nederland), public domain, downloaded from `https://api.pdok.nl/rvo/natura2000/ogc/v1`. These are protected-area boundaries, not UAS zones from the AIP file.

Temporary restrictions are not in this repository. They change by NOTAM and have no static national file.
