# A re-usable data explorer based on the NYC Environment and Health Data Portal
This repository contains re-usable code that you can use to build your own Data Explorer - an embeddable web application that lets you add datasets so that users can browse and visualize data. 

## Getting started
You will need to:
- Install hugo and npm
- Install this repository's dependencies via `npm install`

## The basics
In the terminal, you can preview this by entering the command `hugo serve --environment production`. Hugo will print to the terminal a local URL where you can preview this - likely something like `https://localhost1313`.

To build the site, the command `hugo --environment production` will assemble the site to the `/docs` folder.

## How this works
This Data Explorer will display neighborhood-level data with the following views:
- Table
- Map
- Trend
- Correlates (including disparities)

It requires:
- A file called `metadata.json` that includes important metadata about your indicators. These include: numeric IDs, names and descriptions, and flags for which views should be displayed in the Data Explorer.
- Individual indicator data files, `[numericID].json`.
- Geography files for each geography you use.
- `comparisons.json` which provides metadata for the Trend chart's 'comparison' function, which displays similar measures from different indicators. 

## Worth noting
This repository likely has a bunch of extra code. We have taken our product and simplified it a lot, but there is further simplication that can happen. 


https://busy-detergent.cloudvent.net/data-explorer/economic-conditions/?id=103#display=summary