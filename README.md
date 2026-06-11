# TuneThere

Drop a pin on a map, find nearby FM/AM radio, and tune in — a worldwide radio receiver in your browser, art-directed like an '80s digital dashboard.

**Live:** https://tunethere.com

## Features
- **Map-first** — tap anywhere or search a place to pull in local stations
- **Tuner** — a tactile dial with co-channel de-duplication (one station per frequency, nearest to your pin) and Web Audio static between stations
- **List** + now-playing dock, dark/light themes, keyboard + screen-reader support
- **Sports** — see which game is "on the radio" (MLB, NHL, NBA, MLS, with NFL/EPL to come) and tune the team's flagship station

## Tech
A single, self-contained `index.html` — no build step.
- Map: [MapLibre GL](https://maplibre.org) + [CARTO](https://carto.com) basemaps
- Stations: [Radio Browser](https://www.radio-browser.info)
- Geocoding: [OpenStreetMap Nominatim](https://nominatim.openstreetmap.org)
- Sports schedules: MLB Stats API + ESPN
- 7-segment readout: [DSEG](https://github.com/keshikan/DSEG)

## Run locally
Any static server works, e.g.:

```sh
python -m http.server 5193
```

then open http://localhost:5193

## Deploy
Static site — deploys to Vercel (or any static host) with zero configuration.

## Credits
Stations via Radio Browser · Places via OpenStreetMap · Map tiles via CARTO
