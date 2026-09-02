# GTFS Transit Feeds

This repository hosts GTFS feeds for public transport operators in Lombardy, Italy.

The feeds are maintained with a focus on accuracy, consistency, data quality and up-to-date operational information, with particular attention to regional conventions and best practices for transit data.

## Available Feeds

| Operator                                     | GTFS Feed                                                                          |
| -------------------------------------------- | ---------------------------------------------------------------------------------- |
| Autolinee Sabba                              | [gtfs_sabba.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_sabba.zip)           |
| Automobilistica Perego                       | [gtfs_perego.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_perego.zip)         |
| Autonoleggi Bonomi                           | [gtfs_bonomi.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_bonomi.zip)         |
| Autoservizi Gelmi                            | [gtfs_gelmi.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_gelmi.zip)           |
| Autoservizi La Valle                         | [gtfs_lavalle.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_lavalle.zip)       |
| Autotrasporti Rainoldi & C.                  | [gtfs_rainoldi.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_rainoldi.zip)     |
| CTB - Cooperativa Trasporti Bormio           | [gtfs_ctb.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_ctb.zip)               |
| FNM Autoservizi Brescia                      | [gtfs_fnma_bs.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_fnma_bs.zip)       |
| Gianolini Servizi e Trasporti                | [gtfs_gianolini.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_gianolini.zip)   |
| LineeLecco                                   | [gtfs_lineelecco.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_lineelecco.zip) |
| SAI - Società Autolinee Interprovinciali     | [gtfs_sai.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_sai.zip)               |
| SAV - Società Autoservizi Visinoni           | [gtfs_sav.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_sav.zip)               |
| STPS - Società Trasporti Pubblici di Sondrio | [gtfs_stps.zip](https://shoummobar.github.io/gtfs-feeds/gtfs_stps.zip)             |

## Data Quality

The GTFS feeds are based on the latest available operational data and are carefully processed with quality and consistency in mind.

They follow relevant regional stop naming conventions and GTFS best practices, and contain the necessary data required for a complete and reliable transit feed.

Before publication, the data is carefully reviewed and cleaned to ensure accurate and consistent information while avoiding unnecessary duplication, inconsistencies or clutter in the passenger-facing experience.

> **Note regarding SAI - Società Autolinee Interprovinciali:** Although the data in this feed is up to date, the underlying data structure has not yet undergone the same level of structural revision and UI/UX refinement applied to the other feeds. As a result, some information in this particular feed may still appear somewhat cluttered or inconsistent from a passenger-facing perspective.
## Updates

Feeds are updated whenever new or revised operational data becomes available.

The existing URLs will be retained when feeds are updated, allowing consuming platforms to continuously access the latest available version without requiring changes to their feed configuration.

## GTFS

All feeds are provided as standard GTFS ZIP archives and are intended for use by platforms and services supporting the [General Transit Feed Specification (GTFS)](https://gtfs.org/).

## GTFS-RT Alerts

Realtime service alerts are provided as individual GTFS-Realtime Protocol Buffer (`.pb`) feeds, with one feed available for each operator.

| Operator                                     | GTFS-RT Alerts                                                                     |
| -------------------------------------------- | ---------------------------------------------------------------------------------- |
| Autolinee Sabba                              | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/sabba/alerts.pb)      |
| Automobilistica Perego                       | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/perego/alerts.pb)     |
| Autonoleggi Bonomi                           | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/bonomi/alerts.pb)     |
| Autoservizi Gelmi                            | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/gelmi/alerts.pb)      |
| Autoservizi La Valle                         | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/lavalle/alerts.pb)    |
| Autotrasporti Rainoldi & C.                  | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/rainoldi/alerts.pb)   |
| CTB - Cooperativa Trasporti Bormio           | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/ctb/alerts.pb)        |
| FNM Autoservizi Brescia                      | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/fnma_bs/alerts.pb)    |
| Gianolini Servizi e Trasporti                | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/gianolini/alerts.pb)  |
| LineeLecco                                   | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/lineelecco/alerts.pb) |
| SAI - Società Autolinee Interprovinciali     | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/sai/alerts.pb)        |
| SAV - Società Autoservizi Visinoni           | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/sav/alerts.pb)        |
| STPS - Società Trasporti Pubblici di Sondrio | [alerts.pb](https://shoummobar.github.io/gtfs-feeds/realtime/stps/alerts.pb)       |

Each feed contains the active service alerts for the corresponding operator and is generated directly by the console as a GTFS-Realtime Protocol Buffer feed.

The corresponding `alerts.json` file is used as the readable shared source for managing and synchronizing alerts, while `alerts.pb` is the binary feed intended for realtime consumers. The code explicitly filters the alerts so that only enabled alerts are included in the generated protobuf feed.

---

**Accurate · Consistent · Current · Clean · Reliable**
