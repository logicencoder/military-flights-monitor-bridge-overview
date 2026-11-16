# Military Flights Monitor

![Military Flights Monitor live ADS-B map with aircraft details](assets/military-flights-monitor-live-map-aircraft-details.png)

Publicly visible aircraft activity can be difficult to explore in a long list of positions and aircraft identifiers. Military Flights Monitor brings the available military-aircraft observations into a live map console with a searchable board and activity views, making it easier to explore the activity that is actually being broadcast.

## Tech stack

| Layer | Technologies |
|---|---|
| Core stack | Python; PHP; WordPress; JavaScript |

## Explore the live map

The **Live map** is the main view. A side panel lists every aircraft with a position, with search and sorting; click one on the map or in the list and the panel turns into its detail card: altitude, speed, track, squawk, last fix, airframe, country of registration, why it ranks where it does and its current flight path. Follow keeps it centred, and Copy link shares exactly that aircraft. The legend filters categories, and the Trails and Density layers show every current flight path and where traffic was seen over the last two weeks.

Between updates, aircraft move by projecting their last reported speed and track for at most a minute; older positions are drawn faded.

## Review the board

The **Board** lists every tracked military aircraft, including those without a position, with callsign, category, airframe, registration, country, altitude, speed and interest score. Columns sort, filters narrow the list, a row opens the aircraft on the map, and the current view exports to CSV. Emergency squawks (7500, 7600 and 7700) are highlighted.

## Read the activity

**Activity** shows how many aircraft are airborne, ops tempo per hour over the last 48 hours, the category mix, the most common airframe types, altitude bands and countries. **Intel** lists aircraft holding station, pairs flying in close company (possible refuelling or formations), airframes first seen in the last day and the most-tracked airframes. **About** explains categories, scores and the data pipeline and shows the feed's current status.

## Understand the coverage

The product uses publicly available ADS-B observations from adsb.fi. Only aircraft present in that source can appear; many aircraft and operations are not represented. The monitor is a view of available broadcasts, not a complete account of military aviation.

The source's coverage sets the boundary of the picture. Use the monitor to explore the observations it contains while retaining that boundary when sharing or interpreting a result.


---

Private code: [military-flights-monitor-bridge](https://github.com/logicencoder/military-flights-monitor-bridge)

See [REPOS.md](REPOS.md) for related repositories.

**[Logic Encoder](https://logicencoder.com)** · [GitHub](https://github.com/logicencoder) · [Contact](https://logicencoder.com/contact/)

