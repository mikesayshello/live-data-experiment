# Live Data Experiment

A single-page website that shows live data for Portland, Oregon, with a silly sense of humor. It is one file (`index.html`) with no frameworks and nothing to install.

**Live site:** https://mikesayshello.github.io/live-data-experiment/

## What it shows

- Current time, as a digital clock and an analog clock with a smooth second hand
- Sunrise and sunset, with how long until the next one (or how long ago it happened)
- Moon phase, next full and new moon, and next moonrise and moonset
- Rainfall for the last 1 to 144 hours, plus a chart of rain in each single hour
- Barometric pressure and trend over the last 48 hours
- Price of silver
- A list of all my public GitHub projects at the bottom
- Funny captions that change every minute

## Where the data comes from

| Data | Source |
| --- | --- |
| Rainfall and pressure | [Open-Meteo](https://open-meteo.com/) (modeled data, not a rain gauge or a barometer) |
| Silver price | [gold-api.com](https://gold-api.com/) |
| GitHub projects | GitHub public API |
| Sun and moon times | Calculated on the page, no internet needed (moon times are accurate to about 15 minutes) |

Rainfall, pressure, and GitHub refresh every 10 minutes. Silver refreshes every 5 minutes. If a source fails, the page shows the reason instead of a blank spot.

## Run it

Open `index.html` in any browser. An internet connection is needed for rainfall, pressure, silver, and the GitHub list.

## Put it on GitHub Pages

1. Upload `index.html` to the main folder of a public repo.
2. Go to **Settings > Pages**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, and save.
3. Open `https://USERNAME.github.io/REPO/` after 1 to 2 minutes.

## Notes

- To change the city, edit the latitude and longitude in the Open-Meteo links and the time zone in the page.
- The file name must be lowercase `index.html`.
