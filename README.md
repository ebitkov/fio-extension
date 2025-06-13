# FIO Extension

This repository hosts additional CSV endpoints for the already great [FIO Community API](https://doc.fnar.net/)
for [Prosperous Universe](https://prosperousuniverse.com/).

## Endpoints

### Planets

#### Index

https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/index.csv

An index of all planets, including their natural ID, name and distance to the different CX.

#### Regional

Antares: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/antares.csv

This aggregated list displays details about environmental conditions, current population, current COGC and player base
count of planets in the Antares region.

#### Player Sites

https://github.com/ebitkov/fio-extension/tree/main/csv/planet-sites

Daily aggregation of player bases on a planet. Planetary infrastructure (like CoG Center, warehouses, etc.) are already
excluded. Only planets with at least one player base are present in the list. If there is no file for a planet, then
there is probably nobody living there.

### Population Consumption Index

AI1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/AI1.csv

An aggregated list, which displays the costs of 100 workers per day over time. The costs where calculated using the FIO
`/csv/prices` endpoint, by using the average of the ask and bid price of a given consumable.

### Sheets

https://docs.google.com/spreadsheets/d/1TldTCpqeFSdPKbMz7fV7QXBth4b8y1yvZnouotzGqBE/edit?usp=sharing

Displays the data as line graphs. The timeframe can be configured, and it calculates the overall costs increase over the
set time.

## How is the data collected?

There is a secondary private repository hosted on GitHub, which runs daily and
weekly [actions scripts](https://github.com/features/actions) to collect and
aggregate the data from FIO and commit it to this repository.
