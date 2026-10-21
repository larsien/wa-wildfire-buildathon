# Washington State Wildfire — Infrastructure Damage Analysis

Interactive maps and data analysis for Washington State wildfires and infrastructure damage, built for the WA Wildfire Buildathon.

## Files

### 📊 Data
| File | Description |
|------|-------------|
| `DNR_Fire_Statistics_2008_-_Present.csv` | WA DNR fire statistics 2008–2026 (30,521 incidents) |
| `2026_fire_infra_damage.csv` | 2026 fires × infrastructure damage analysis (powerlines + roads) |
| `2026_fire_powerline_damage.csv` | 2026 fires × HIFLD powerline intersection analysis |

### 🗺️ Maps
| File | Description |
|------|-------------|
| `wa_wildfire_map.html` | Interactive WA statewide wildfire map (2008–2026, 30k+ points) |
| `spokane_infra_damage_map_en.html` | Spokane Complex Fire (Aug 2026) infrastructure damage map — real HIFLD powerline data |
| `spokane_infra_damage_map.html` | Same map in Korean |

## Data Sources
- **WA DNR Fire Statistics**: [WA DNR GIS](https://gis.dnr.wa.gov)
- **Power Transmission Lines**: [HIFLD Open Data](https://hifld-geoplatform.opendata.arcgis.com) via ArcGIS REST API
- **Base Maps**: ESRI, CARTO, Google Maps, OpenStreetMap (all no API key required)

## Infrastructure Damage Summary (2026 Season)
- **322** fires analyzed
- **46** fires within range of transmission lines
- **121** powerline segment intersections
- **HIGH risk** fires (5+ powerline hits): 6
- Key utilities affected: Avista Corp, Inland Power & Light, Bonneville Power Administration

## How to Run
Open any `.html` file directly in a browser — no server or API key needed.

## Sharing
```bash
# Local network share
cd wa-wildfire-buildathon
python3 -m http.server 8080
# → http://YOUR_LOCAL_IP:8080/wa_wildfire_map.html
```
