# FIO Extension

This repository hosts additional CSV endpoints for the already great [FIO Community API](https://doc.fnar.net/)
for [Prosperous Universe](https://prosperousuniverse.com/).

## Endpoints

### Building Construction Costs

https://github.com/ebitkov/fio-extension/tree/main/csv/building/construction_costs

Construction cost data for all buildings, including base costs and environmental cost modifiers for different surface types (rocky/gaseous), gravity, temperature, and pressure conditions.

- AI1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/building/construction_costs/AI1.csv

### Planets

#### Index

https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/index.csv

An index of all planets, including their natural ID, name and distance to the different CX.

#### Regional

https://github.com/ebitkov/fio-extension/tree/main/csv/planets

This aggregated list displays details about environmental conditions, current population, population changes, open jobs, COGC status and player base count for planets in each region.

- Antares: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/antares.csv
- Arclight: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/arclight.csv
- Benten: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/benten.csv
- Hortus: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/hortus.csv
- Hubur: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/hubur.csv
- Moria: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/planets/moria.csv

#### Player Sites

https://github.com/ebitkov/fio-extension/tree/main/csv/planet-sites

Daily aggregation of player bases on a planet. Planetary infrastructure (like CoG Center, warehouses, etc.) are already
excluded. Only planets with at least one player base are present in the list. If there is no file for a planet, then
there is probably nobody living there.

### Player Count

https://github.com/ebitkov/fio-extension/tree/main/csv/player/count

Daily aggregation of player counts per region, tracking total bases and unique players over time.

- Antares: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/antares.csv
- Arclight: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/arclight.csv
- Benten: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/benten.csv
- Hortus: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/hortus.csv
- Hubur: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/hubur.csv
- Moria: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/player/count/moria.csv

### Population Consumption Index

https://github.com/ebitkov/fio-extension/tree/main/csv/population-consumption-index

An aggregated list, which displays the costs of 100 workers per day over time. The costs were calculated using the FIO
`/csv/prices` endpoint, by using the average of the ask and bid price of a given consumable. Data includes per-workforce-type costs and individual consumable prices.

- AI1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/AI1.csv
- CI1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/CI1.csv
- CI2: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/CI2.csv
- IC1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/IC1.csv
- NC1: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/NC1.csv
- NC2: https://raw.githubusercontent.com/ebitkov/fio-extension/refs/heads/main/csv/population-consumption-index/NC2.csv

## How is the data collected?

There is a secondary private repository hosted on GitHub, which runs daily and
weekly [actions scripts](https://github.com/features/actions) to collect and
aggregate the data from FIO and commit it to this repository.
