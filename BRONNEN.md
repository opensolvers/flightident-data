# Bronnen

Herkomst van de bestanden in deze repo. Bij een nieuwe download: datum, URL en aantal gebieden hier bijwerken.

## UAS-zones Nederland

| | |
| --- | --- |
| Bestand | `nl/uas-zones.json` |
| Uitgave | 22 juli 2024, 09:07 (`UASZoneVersion 2024-07-22 09:07`) |
| Oorspronkelijke bestandsnaam | `Alle statische zonering en andere gebieden in ED269 format - 22juli2024.JSON` |
| Laatst gewijzigd op de server | 24 juli 2024, 10:26 UTC |
| Formaat | EUROCAE ED-269 JSON, ongewijzigd overgenomen |
| Inhoud | 774 zones: 10 prohibited, 51 authorisation required, 713 conditional |
| Gekopieerd | 3 oktober 2026 |

Publicatie: AIP Nederland, ENR 5.3, onderdeel 1.5, AIRAC AMDT 10-2026 (geldig vanaf 1 oktober 2026). De informatie moet openbaar zijn op grond van artikel 15 van verordening (EU) 2019/947.

- AIP-pagina: <https://eaip.lvnl.nl/web/eaip/AIRAC%20AMDT%2010-2026_2026_10_01/eAIP/EH-ENR%205.3-en-GB.html>
- Download: <https://www.nieuwsienw.nl/api/documents/downloadfile?sectionid=178144&fileid=1650029&forcedownload=true>

## Afgeleide gebiedsbestanden

Deze GeoJSON-bestanden zijn geen aparte bron. Ze zijn op 3 oktober 2026 gesplitst uit `nl/uas-zones.json`. Cirkels zijn benaderd met 64 punten. De regeltekst per zone komt uit het bronbestand.

| Bestand | Aantal | Groep in de bron |
| --- | --- | --- |
| `nl/gebieden/verboden.geojson` | 10 | `PROHIBITED` |
| `nl/gebieden/beveiligd.geojson` | 338 | beveiligde gebieden, vitale processen en beveiligingsverboden |
| `nl/gebieden/industrie.geojson` | 270 | industrie en haven met risico op zware ongevallen |
| `nl/gebieden/vliegvelden.geojson` | 43 | nabijheid van vliegvelden, inclusief CTR’s |
| `nl/gebieden/defensie.geojson` | 67 | defensiegebieden, inclusief zones met militaire toestemming |
| `nl/gebieden/helikopter.geojson` | 23 | landingsplaatsen van trauma- en reddingshelikopters |
| `nl/gebieden/laagvlieg.geojson` | 23 | laagvlieggebieden en blusoefengebieden |

Overzicht van de regeltekst: `nl/gebieden/index.json`.

## Natura 2000

| | |
| --- | --- |
| Bestand | `nl/gebieden/natura2000.geojson` |
| Aanbieder | Rijksdienst voor Ondernemend Nederland, via PDOK |
| Dienst | OGC API Features, collectie `natura2000` |
| URL | <https://api.pdok.nl/rvo/natura2000/ogc/v1> |
| Licentie | Public Domain Mark 1.0 |
| Coördinaten | CRS84, lengtegraad dan breedtegraad |
| Inhoud | 209 gebieden |
| Gedownload | 3 oktober 2026 |

Dit zijn de grenzen van de Natura 2000-gebieden. Het is geen UAS-zone uit AIP ENR 5.3.

## Niet opgenomen

Tijdelijke beperkingen wijzigen via een NOTAM en hebben geen vast landelijk bestand. Andere natuurgebieden dan Natura 2000 hebben geen enkele landelijke open set.
