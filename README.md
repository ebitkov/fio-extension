# FIO Extension

This repository hosts additional CSV endpoints for the already great [FIO Community API](https://doc.fnar.net/)
for [Prosperous Universe](https://prosperousuniverse.com/).

## Endpoints

### Planet Index

https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/index.csv

An index of all planets, including their natural ID, name and distance to the different CX.

### Planets of a Region

Antares: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/antares.csv

This aggregated list displays details about environmental conditions, current population, current COGC and player base
count of planets in the Antares region.

### Population Consumption Index

AI1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/AI1.csv

An aggregated list, which displays the costs of 100 workers per day over time. The costs where calculated using the FIO
`/csv/prices` endpoint, by using the average of the ask and bid price of a given consumable.

### Sheets

https://docs.google.com/spreadsheets/d/1TldTCpqeFSdPKbMz7fV7QXBth4b8y1yvZnouotzGqBE/edit?usp=sharing

Displays the data as line graphs. The timeframe can be configured, and it calculates the overall costs increase over the
set time.
