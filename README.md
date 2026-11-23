<p align="center"><img src="assets/banner.svg" width="100%" alt="Indonesia API endpoints: 22,516 API endpoints passed a keyless data call"></p>

# 🇮🇩 Indonesia API endpoints

**22,516 API endpoints filed under country code ID that answered a keyless GET with a data body. For agent and app builders.**

<p align="center"><a href="#files"><img src="https://img.shields.io/badge/endpoints-22%2C516-6366F1" alt="endpoints: 22,516"></a> <a href="#columns-and-tags"><img src="https://img.shields.io/badge/keyless%20JSON-22%2C516-6366F1" alt="keyless JSON: 22,516"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/services-59-0F172A" alt="services: 59"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/country-ID-EA580C" alt="country: ID"></a> <a href="LICENSE"><img src="https://img.shields.io/badge/licence-CC%20BY%204.0-0F172A" alt="licence: CC BY 4.0"></a></p>

<p align="center"><a href="#whats-in-it-for-you">What's in it</a> · <a href="#for-ai-agents">For AI agents</a> · <a href="#quick-start">Quick start</a> · <a href="#test-it-yourself">Test it yourself</a> · <a href="#files">Files</a> · <a href="#licence-and-credit">Licence</a> · <a href="#part-of-10m-api-endpoints-for-ai-agents">More packs</a></p>

This repository holds a 1,000-row sample and the services list; the full list of 22,516 endpoints is one download from the [latest release](https://github.com/agentpopulation/22k-indonesia-apis-for-agents/releases/latest).

**Endpoints filed under country code ID, for building an agent or app for Indonesia.** Regency statistics tables from the Lamongan open-data portal (farm output, hospital beds, budgets, population by district) as JSON, plus a few map layers, as URLs that answered with no key on their test date.

Selection rule: rows where `country is ID AND format is json`, less the rows that a leave-out rule drops (each counted under Known limits).

22,444 of these 22,516 rows match the focus rule (below); the others are in the pack by the selection rule only, and Known limits says what they are.

## In plain words

**What is an API endpoint?** An API endpoint is one web address that a program can ask for data, for example the latest reading at one weather station. A single service, such as a national weather agency, can have thousands of endpoints: one per station, city or dataset. This pack counts endpoints, not separate services.

**What does "passed a data call" mean?** On the date shown in each row, AgentPopulation sent one plain request to that address, with no password or key, and got a non-empty data body back (JSON, CSV, XML or a file): not an error page and not an empty result. Some bodies describe a dataset rather than hold its values; see Known limits. It shows the address answered with data on that day. It is not a promise that it answers today, and licences and usage limits were not reviewed.

## What's in it for you

Four ways to use this pack. Each bucket gives a count, a filter you can apply to the CSV, one example that passed, and a list of recommended starting points with the rule that picked them. Buckets overlap; a row can fit more than one.

Examples, recommended lists and the preview are drawn from rows that match this pack's focus rule, so a row that the selection rule put in this pack but that is about something else is not shown as a starting point. Counts cover the whole bucket.

<details>
<summary>The focus rule</summary>

Focus rule: `NOT title matches /(?<![a-z])(test|tests|testing|draft|drafts|copy|sample|samples|demo|untitled|scratch|temp|tmp|delete|deleteme|practice|dummy|example|training)(?![a-z])|final_final|\d{7,}/i`

</details>

### 🤖 Agent tools: Keyless JSON layers and tables an agent can call (Indonesia)

**22,516** endpoints from 59 services · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.

924 of these are map-layer queries that asked for a few records (`resultRecordCount`); add a where clause or a geometry to ask about one place, and page through for the whole layer.

Start with: `tags has agent-ready`

Example: [01\_TowerPrediction](https://services-ap1.arcgis.com/wYEzTTDGwSuQQW1R/ArcGIS/rest/services/01_TowerPrediction/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · ArcGIS Online layers (services-ap1.arcgis.com, org wYEzTTDGwSuQQW1R) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and are tagged `agent-ready` (no key sent in the test call, JSON body, passed a data call). Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Sample preference in this bucket: `url matches //query\?/i`. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Portal Data Lamongan (data.lamongankab.go.id) | 21,592 | 21,592 | ID | json | [Bantuan Hukum - Periode Juni 2023 - Dat…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) (2026-11-16) |
| Conservation International (ArcGIS Online) (services.arcgis.com) | 51 | 51 | ID | json | [AOI Survey Biodiversity](https://services.arcgis.com/bL1WyMoaiBW4etad/arcgis/rest/services/AOI_Survey_Biodiversity/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Hub Community (ArcGIS Online) (services8.arcgis.com) | 51 | 51 | ID | json | [AH\_Boundary](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Three Rivers Waterkeeper (ArcGIS Online) (services1.arcgis.com) | 35 | 35 | ID | json | [2024\_Swim\_Guide\_Working\_Data\_\_\_tributar…](https://services1.arcgis.com/t1SiaMcpdmU5aHVK/ArcGIS/rest/services/2024_Swim_Guide_Working_Data___tributariesGIS/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Tiger Team (ArcGIS Online) (services8.arcgis.com) | 25 | 25 | ID | json | [Agrinas\_HGU\_WFL1](https://services8.arcgis.com/mpSDBlkEzjS62WgX/arcgis/rest/services/Agrinas_HGU_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| PT GEOJAYA TEHNIK (ArcGIS Online) (services6.arcgis.com) | 11 | 11 | ID | json | [GD IKN UPDATE](https://services6.arcgis.com/UumfQ6GRw4Re8PJZ/arcgis/rest/services/GD_IKN_UPDATE/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Geonet Infomedia (ArcGIS Online) (services6.arcgis.com) | 5 | 5 | ID | json | [Batas Administrasi](https://services6.arcgis.com/hdfh5OsOlUgKLttT/arcgis/rest/services/Batas_Administrasi/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Good Forest Indonesia (ArcGIS Online) (services2.arcgis.com) | 5 | 5 | ID | json | [Applied\_Nucleation](https://services2.arcgis.com/Qkfnoxl9DbwkzQ25/ArcGIS/rest/services/Applied_Nucleation/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 📱 App features: Tables and layers to show in an app (Indonesia)

**22,516** endpoints from 59 services · Show a regency table as a card or a chart, with the period and the source.

Start with: the whole pack

Example: [Bantuan Hukum - Periode Juni 2023 - Data JSON Jun…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) · Portal Data Lamongan · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Portal Data Lamongan (data.lamongankab.go.id) | 21,592 | 21,592 | ID | json | [Bantuan Hukum - Periode Juni 2023 - Dat…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) (2026-11-16) |
| Conservation International (ArcGIS Online) (services.arcgis.com) | 51 | 51 | ID | json | [AOI Survey Biodiversity](https://services.arcgis.com/bL1WyMoaiBW4etad/arcgis/rest/services/AOI_Survey_Biodiversity/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Hub Community (ArcGIS Online) (services8.arcgis.com) | 51 | 51 | ID | json | [AH\_Boundary](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Three Rivers Waterkeeper (ArcGIS Online) (services1.arcgis.com) | 35 | 35 | ID | json | [2024\_Swim\_Guide\_Working\_Data\_\_\_tributar…](https://services1.arcgis.com/t1SiaMcpdmU5aHVK/ArcGIS/rest/services/2024_Swim_Guide_Working_Data___tributariesGIS/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Tiger Team (ArcGIS Online) (services8.arcgis.com) | 25 | 25 | ID | json | [Agrinas\_HGU\_WFL1](https://services8.arcgis.com/mpSDBlkEzjS62WgX/arcgis/rest/services/Agrinas_HGU_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| PT GEOJAYA TEHNIK (ArcGIS Online) (services6.arcgis.com) | 11 | 11 | ID | json | [GD IKN UPDATE](https://services6.arcgis.com/UumfQ6GRw4Re8PJZ/arcgis/rest/services/GD_IKN_UPDATE/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Geonet Infomedia (ArcGIS Online) (services6.arcgis.com) | 5 | 5 | ID | json | [Batas Administrasi](https://services6.arcgis.com/hdfh5OsOlUgKLttT/arcgis/rest/services/Batas_Administrasi/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Good Forest Indonesia (ArcGIS Online) (services2.arcgis.com) | 5 | 5 | ID | json | [Applied\_Nucleation](https://services2.arcgis.com/Qkfnoxl9DbwkzQ25/ArcGIS/rest/services/Applied_Nucleation/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧠 Grounding and data pipelines: Regency statistics tables for scheduled loads (Indonesia)

**22,516** endpoints from 59 services · Load the regency tables on a schedule into your own store, so an agent can cite a dated source.

Start with: the whole pack

Example: [Bantuan Hukum - Periode Juni 2023 - Data JSON Jun…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) · Portal Data Lamongan · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Portal Data Lamongan (data.lamongankab.go.id) | 21,592 | 21,592 | ID | json | [Bantuan Hukum - Periode Juni 2023 - Dat…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) (2026-11-16) |
| Conservation International (ArcGIS Online) (services.arcgis.com) | 51 | 51 | ID | json | [AOI Survey Biodiversity](https://services.arcgis.com/bL1WyMoaiBW4etad/arcgis/rest/services/AOI_Survey_Biodiversity/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Hub Community (ArcGIS Online) (services8.arcgis.com) | 51 | 51 | ID | json | [AH\_Boundary](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Three Rivers Waterkeeper (ArcGIS Online) (services1.arcgis.com) | 35 | 35 | ID | json | [2024\_Swim\_Guide\_Working\_Data\_\_\_tributar…](https://services1.arcgis.com/t1SiaMcpdmU5aHVK/ArcGIS/rest/services/2024_Swim_Guide_Working_Data___tributariesGIS/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Tiger Team (ArcGIS Online) (services8.arcgis.com) | 25 | 25 | ID | json | [Agrinas\_HGU\_WFL1](https://services8.arcgis.com/mpSDBlkEzjS62WgX/arcgis/rest/services/Agrinas_HGU_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| PT GEOJAYA TEHNIK (ArcGIS Online) (services6.arcgis.com) | 11 | 11 | ID | json | [GD IKN UPDATE](https://services6.arcgis.com/UumfQ6GRw4Re8PJZ/arcgis/rest/services/GD_IKN_UPDATE/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Geonet Infomedia (ArcGIS Online) (services6.arcgis.com) | 5 | 5 | ID | json | [Batas Administrasi](https://services6.arcgis.com/hdfh5OsOlUgKLttT/arcgis/rest/services/Batas_Administrasi/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Good Forest Indonesia (ArcGIS Online) (services2.arcgis.com) | 5 | 5 | ID | json | [Applied\_Nucleation](https://services2.arcgis.com/Qkfnoxl9DbwkzQ25/ArcGIS/rest/services/Applied_Nucleation/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧪 Evals and testing: Varied responses to test tool calls and parsers

**22,516** endpoints · 59 services · country ID · 1 format · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

Start with: the whole pack

Example: [Bantuan Hukum - Periode Juni 2023 - Data JSON Jun…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) · Portal Data Lamongan · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack that returned the most different formats, then the most endpoints that passed a data call, then by name: a mix of response shapes to test parsers and tool calls. Here the services returned 1 format each, so the order comes down to endpoint counts. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| Portal Data Lamongan (data.lamongankab.go.id) | 21,592 | 21,592 | ID | json | [Bantuan Hukum - Periode Juni 2023 - Dat…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) (2026-11-16) |
| Conservation International (ArcGIS Online) (services.arcgis.com) | 51 | 51 | ID | json | [AOI Survey Biodiversity](https://services.arcgis.com/bL1WyMoaiBW4etad/arcgis/rest/services/AOI_Survey_Biodiversity/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Hub Community (ArcGIS Online) (services8.arcgis.com) | 51 | 51 | ID | json | [AH\_Boundary](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Three Rivers Waterkeeper (ArcGIS Online) (services1.arcgis.com) | 35 | 35 | ID | json | [2024\_Swim\_Guide\_Working\_Data\_\_\_tributar…](https://services1.arcgis.com/t1SiaMcpdmU5aHVK/ArcGIS/rest/services/2024_Swim_Guide_Working_Data___tributariesGIS/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Tiger Team (ArcGIS Online) (services8.arcgis.com) | 25 | 25 | ID | json | [Agrinas\_HGU\_WFL1](https://services8.arcgis.com/mpSDBlkEzjS62WgX/arcgis/rest/services/Agrinas_HGU_WFL1/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| PT GEOJAYA TEHNIK (ArcGIS Online) (services6.arcgis.com) | 11 | 11 | ID | json | [GD IKN UPDATE](https://services6.arcgis.com/UumfQ6GRw4Re8PJZ/arcgis/rest/services/GD_IKN_UPDATE/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Geonet Infomedia (ArcGIS Online) (services6.arcgis.com) | 5 | 5 | ID | json | [Batas Administrasi](https://services6.arcgis.com/hdfh5OsOlUgKLttT/arcgis/rest/services/Batas_Administrasi/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) (2026-11-16) |
| Good Forest Indonesia (ArcGIS Online) (services2.arcgis.com) | 5 | 5 | ID | json | [Applied\_Nucleation](https://services2.arcgis.com/Qkfnoxl9DbwkzQ25/ArcGIS/rest/services/Applied_Nucleation/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

The same lists are in [recommended.json](recommended.json), ready for an agent to load.

## Questions an agent can answer with this pack

- What does a Lamongan regency table report for one period? Try [Bantuan Hukum - Periode Juni 2023 - Data JSON Jun…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) (Portal Data Lamongan, passed 2026-11-16).
- What rainfall map layers does the national weather agency serve? Try [Peta\_Curah\_Hujan\_dan\_Hari\_Hujan](https://gis.bmkg.go.id/arcgis/rest/services/Peta_Curah_Hujan_dan_Hari_Hujan/MapServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Bmkg, passed 2026-11-16).
- Which boundary layers does Hub Community publish for Indonesia? Try [AH\_Boundary](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Hub Community (ArcGIS Online), passed 2026-11-16).

## What "passed a data call" means

> [!NOTE]
> On the date in `last_tested` (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The `format` column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16 Nov 2026; snapshot 16 Nov 2026.

## For AI agents

Start from keyless JSON endpoints (`agent-ready`). The code below loads `recommended.json` and calls the first recommended service in the Agent tools bucket, with a timeout (`node examples/agent-start.mjs --recommended`). With no argument, `node examples/agent-start.mjs` calls the most recently tested agent-ready row of the sample; pass a `.csv` or `.csv.gz` path to use that file instead. See [examples/agent-start.mjs](examples/agent-start.mjs).

```js
// Node 18+. Loads recommended.json (the local copy, or the raw file on GitHub) and calls one keyless JSON endpoint.
import fs from 'node:fs';

const RAW = 'https://raw.githubusercontent.com/agentpopulation/22k-indonesia-apis-for-agents/main/recommended.json';
const rec = fs.existsSync('recommended.json')
  ? JSON.parse(fs.readFileSync('recommended.json', 'utf8'))
  : await (await fetch(RAW)).json();

const pick = rec.buckets.find((b) => b.id === 'agent').services[0];
try {
  const res = await fetch(pick.sample_url, {
    headers: { 'User-Agent': 'agent-example/1.0' },
    signal: AbortSignal.timeout(15000),
  });
  console.log(pick.service, res.status, res.headers.get('content-type'));
  console.log((await res.text()).slice(0, 300));
} catch (err) {
  console.log(`did not answer now; last passed ${pick.sample_last_tested} (${err.message})`);
}
```

How an agent picks an endpoint:

1. Filter to `agent-ready` and your country or topic.
2. Prefer the newest `last_tested` and the larger services.
3. Call with a timeout and check the body before you use it.

## Quick start

The examples run against the sample in `data/` out of the box (1,000 rows). Each takes an optional path to a `.csv` or `.csv.gz` file instead.

```bash
git clone https://github.com/agentpopulation/22k-indonesia-apis-for-agents.git
cd 22k-indonesia-apis-for-agents
python examples/quickstart.py
node examples/quickstart.mjs
node examples/agent-start.mjs
```

Full list: download `Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (22,516 rows, 1.4 MB) from [releases/latest](https://github.com/agentpopulation/22k-indonesia-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

```bash
gunzip Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz
python examples/quickstart.py Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
node examples/quickstart.mjs Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
```

### curl

Quote the URL: some contain commas.

```bash
curl -sL "https://raw.githubusercontent.com/agentpopulation/22k-indonesia-apis-for-agents/main/data/Indonesia_API_Endpoints_AgentPopulation_Sample.csv" | head -n 4
curl -s --max-time 15 "https://services-ap1.arcgis.com/wYEzTTDGwSuQQW1R/ArcGIS/rest/services/01_TowerPrediction/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json" | head -c 600
```

### Python

Standard library only: [examples/quickstart.py](examples/quickstart.py) reads the sample, or the path you pass, keeps agent-ready rows and calls the most recently tested one.

<details>
<summary>The code</summary>

```python
# Python 3, standard library only. Run from a clone of this repository:
#   python examples/quickstart.py [path]
# With no path it reads the sample in data/. Pass the full list from the latest release (.csv or .csv.gz) instead.
# Keeps agent-ready rows and calls the most recently tested one.
import csv
import gzip
import os
import re
import sys
import urllib.request

HERE = os.path.dirname(os.path.abspath(__file__))
path = sys.argv[1] if len(sys.argv) > 1 else os.path.join(HERE, "..", "data", "Indonesia_API_Endpoints_AgentPopulation_Sample.csv")
opener = gzip.open if path.endswith(".gz") else open
with opener(path, "rt", newline="", encoding="utf-8") as f:
    rows = list(csv.DictReader(f))

agent = [r for r in rows if "agent-ready" in r["tags"].split("|")]
# Newest test date first; URLs that describe a dataset or a service rather than return values go last.
DESCRIBES = re.compile(r"/erddap/info/|action-report\.json$|[?&]request=getcapabilities|/GeoArea/[^/?]+/List|getFullTableDownloadCSV|hub\.worldpop\.org", re.I)
agent.sort(key=lambda r: r["last_tested"], reverse=True)
agent.sort(key=lambda r: 1 if DESCRIBES.search(r["url"]) else 0)
print(len(rows), "rows,", len(agent), "agent-ready")
if not agent:
    sys.exit(0)

row = agent[0]
req = urllib.request.Request(row["url"], headers={"User-Agent": "agent-example/1.0"})
try:
    with urllib.request.urlopen(req, timeout=15) as res:
        body = res.read(1_000_000).decode("utf-8", "replace")
        print(res.status, res.headers.get("Content-Type"))
        print(body[:300])
except Exception as err:
    print(f"did not answer now; last passed {row['last_tested']} ({err})")
```

</details>

### JavaScript

Reads the sample as JSON because the CSV has quoted commas.

<details>
<summary>The code</summary>

```js
// Node 18+. Reads the sample as JSON (the CSV has quoted commas), local file first.
import fs from 'node:fs';

const FILE = 'data/Indonesia_API_Endpoints_AgentPopulation_Sample.json';
const rows = fs.existsSync(FILE)
  ? JSON.parse(fs.readFileSync(FILE, 'utf8'))
  : await (await fetch('https://raw.githubusercontent.com/agentpopulation/22k-indonesia-apis-for-agents/main/data/Indonesia_API_Endpoints_AgentPopulation_Sample.json')).json();

const row = rows.find((r) => r.tags.includes('agent-ready'));
const res = await fetch(row.url, { headers: { 'User-Agent': 'agent-example/1.0' }, signal: AbortSignal.timeout(15000) });
console.log(res.status, (await res.text()).slice(0, 300));
```

</details>

### Agent tools

[examples/agent-tools.json](examples/agent-tools.json) holds two tool definitions in the shape most tool-calling APIs accept (name, description, JSON Schema); rename `parameters` if yours uses another key. [examples/quickstart.mjs](examples/quickstart.mjs) implements them:

- `find_endpoints` searches the agent-ready rows of the list by words (their format is json). When you load the tools of more than one pack, prefix the names (for example `indonesia_find_endpoints`) so they do not clash.
- `fetch_endpoint` calls one URL, **refuses any URL that is not in the list** and does not follow redirects. The allowlist is built from the CSV, so a URL injected into a prompt is refused.

The same two tools can sit behind an MCP server.

## Test it yourself

Re-test endpoints from the sample with the same rule: HTTP 2xx and a non-empty body that is not an HTML page. Node 18+, no packages.

```bash
node tools/test-endpoints.mjs
```

It tests the first 50 URLs and prints one line: tested, passed, did not pass. Options: a `.csv` or `.csv.gz` path (the full list from the release), `--limit 50`, `--timeout-ms 10000`, `--out results.csv`. The results file holds `url`, `status`, `passed`, `content_type`, `ms` and `checked_at`; a status of `timeout` or `error:<code>` means no HTTP answer came back. It is polite: GET only, no key sent, at most 4 requests in flight, one at a time per listed host, at least 1 second between requests to one listed host, and reading stops once 256 kB of a body is kept. Redirects are followed and may lead to another host. `results.csv` is in `.gitignore`.

## Preview

One row from each of the five largest services among rows that match the focus rule, services with rows that return values first.

| Title | Service | Country | Format | Tested | Link |
|---|---|---|---|---|---|
| Bantuan Hukum - Periode Juni 2023 - Data JSON Juni 2023 | Portal Data Lamongan | ID | json | 2026-11-16 | [data.lamongankab.go.id](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) |
| 01\_TowerPrediction | ArcGIS Online layers (services-ap1.arcgis.com, org wYEzTTDGwSuQQW1R) | ID | json | 2026-11-16 | [services-ap1.arcgis.com](https://services-ap1.arcgis.com/wYEzTTDGwSuQQW1R/ArcGIS/rest/services/01_TowerPrediction/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| 1\_Benua | ArcGIS Online layers (services3.arcgis.com, org VFq4ZNL4ohXxN8gl) | ID | json | 2026-11-16 | [services3.arcgis.com](https://services3.arcgis.com/VFq4ZNL4ohXxN8gl/arcgis/rest/services/1_Benua/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) |
| AOI Survey Biodiversity | Conservation International (ArcGIS Online) | ID | json | 2026-11-16 | [services.arcgis.com](https://services.arcgis.com/bL1WyMoaiBW4etad/arcgis/rest/services/AOI_Survey_Biodiversity/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=5&f=json) |
| AH\_Boundary | Hub Community (ArcGIS Online) | ID | json | 2026-11-16 | [services8.arcgis.com](https://services8.arcgis.com/1v1brwt6r4ooA9mb/ArcGIS/rest/services/AH_Boundary/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |

Browse the 1,000-row sample: [Sample CSV](data/Indonesia_API_Endpoints_AgentPopulation_Sample.csv) · [Sample JSON](data/Indonesia_API_Endpoints_AgentPopulation_Sample.json).

## What's inside

<p align="center"><img src="assets/breakdown.svg" width="100%" alt="Top categories and formats in this pack"></p>

<details>
<summary>Categories: top 8</summary>

| Category | Endpoints | |
|---|---:|---|
| Statistics & Economy | 21,439 | `████████████████████` |
| Navigation & Geo/Maps | 405 | `▍` |
| Government & Open Data | 395 | `▍` |
| Transport & Mobility | 75 | `▏` |
| Finance | 73 | `▏` |
| Environment | 39 | `▏` |
| Energy | 30 | `▏` |
| Weather & Climate | 22 | `▏` |

</details>

Formats: json 22,516

<details>
<summary>Largest services: top 25 of 59</summary>

| Service | Host | Endpoints | Keyless JSON | |
|---|---|---:|---:|---|
| Portal Data Lamongan | data.lamongankab.go.id | 21,592 | 21,592 | `████████████████████` |
| ArcGIS Online layers (services-ap1.arcgis.com, org wYEzTTDGwSuQQW1R) | services-ap1.arcgis.com | 193 | 193 | `▏` |
| ArcGIS Online layers (services3.arcgis.com, org VFq4ZNL4ohXxN8gl) | services3.arcgis.com | 181 | 181 | `▏` |
| ArcGIS Online layers (services-ap1.arcgis.com, org TjPT2JHoHdhHU7cr) | services-ap1.arcgis.com | 70 | 70 | `▏` |
| Conservation International (ArcGIS Online) | services.arcgis.com | 51 | 51 | `▏` |
| Hub Community (ArcGIS Online) | services8.arcgis.com | 51 | 51 | `▏` |
| Three Rivers Waterkeeper (ArcGIS Online) | services1.arcgis.com | 35 | 35 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org f290PpjVVF5Ie2gu) | services7.arcgis.com | 34 | 34 | `▏` |
| ArcGIS Online layers (services6.arcgis.com, org R04lBEmHupGfIw1K) | services6.arcgis.com | 25 | 25 | `▏` |
| Tiger Team (ArcGIS Online) | services8.arcgis.com | 25 | 25 | `▏` |
| ArcGIS Online layers (services-ap1.arcgis.com, org zddIc5NlxDyZbzsT) | services-ap1.arcgis.com | 24 | 24 | `▏` |
| ArcGIS Online layers (services.arcgis.com, org tlJcENMD2zMI0kgn) | services.arcgis.com | 21 | 21 | `▏` |
| ArcGIS Online layers (services8.arcgis.com, org orYEK4i9yXvAYwAZ) | services8.arcgis.com | 17 | 17 | `▏` |
| ArcGIS Online layers (services-ap1.arcgis.com, org wAmT3FNM08kqGino) | services-ap1.arcgis.com | 12 | 12 | `▏` |
| PT GEOJAYA TEHNIK (ArcGIS Online) | services6.arcgis.com | 11 | 11 | `▏` |
| ArcGIS Online layers (services5.arcgis.com, org LtKK0bbgiII9cWQ0) | services5.arcgis.com | 10 | 10 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org AEUtWyWsEA5EGD2t) | services7.arcgis.com | 9 | 9 | `▏` |
| ArcGIS Online layers (services3.arcgis.com, org SGnlfsP6aiCdgBcR) | services3.arcgis.com | 9 | 9 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org arZnhQhtvIXpgVPD) | services7.arcgis.com | 9 | 9 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org icMrlKBWZnnubzc7) | services7.arcgis.com | 9 | 9 | `▏` |
| ArcGIS Online layers (services3.arcgis.com, org 6FjQ0DRWiaCpjd6B) | services3.arcgis.com | 8 | 8 | `▏` |
| ArcGIS Online layers (services-eu1.arcgis.com, org 7BbuBL834vOB5cCY) | services-eu1.arcgis.com | 8 | 8 | `▏` |
| ArcGIS Online layers (services2.arcgis.com, org LvCBNZuwhTWWbvod) | services2.arcgis.com | 8 | 8 | `▏` |
| ArcGIS Online layers (services8.arcgis.com, org TIDaqFGVtcBJNSoQ) | services8.arcgis.com | 8 | 8 | `▏` |
| ArcGIS Online layers (services-ap1.arcgis.com, org vRjNB2A4PDiSDCTH) | services-ap1.arcgis.com | 8 | 8 | `▏` |

</details>

<details>
<summary>Rows per test date: 16 Nov 2026</summary>

| Date (IST) | Endpoints | |
|---|---:|---|
| 2026-11-16 | 22,516 | `████████████████████` |

</details>

## Files

| File | Rows | Size | Use |
|---|---:|---:|---|
| [data/Indonesia_API_Services_AgentPopulation.csv](data/Indonesia_API_Services_AgentPopulation.csv) | 59 | 3.8 kB | One row per service with its endpoint count in this pack |
| [data/Indonesia_API_Endpoints_AgentPopulation_Sample.csv](data/Indonesia_API_Endpoints_AgentPopulation_Sample.csv) | 1,000 | 341.1 kB | The sample: focus-rule rows first, each service in proportion to its share; ArcGIS Online layers count as one service |
| [data/Indonesia_API_Endpoints_AgentPopulation_Sample.json](data/Indonesia_API_Endpoints_AgentPopulation_Sample.json) | 1,000 | 523.9 kB | The same rows as JSON, tags as an array |
| [Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz](https://github.com/agentpopulation/22k-indonesia-apis-for-agents/releases/latest) | 22,516 | 1.4 MB | The full list, gzipped CSV: a download from the latest release, checked by `SHA256SUMS.txt` |
| [tools/test-endpoints.mjs](tools/test-endpoints.mjs) | | | Re-tests endpoints from the sample or the full list |

Sample size: 1,000 rows, which is 1,000 or one third of the pack rounded down, whichever is smaller. Rows that match the focus rule come first. Each service gets rows in proportion to its share of those rows, at least one for the largest services and at most 50% of the sample while other services have rows; ArcGIS Online layers count as one service, whatever their organisation. Within a service, agent-ready rows, rows that return values and the newest test dates come first, and rows are written in turn across services. Service root addresses are placed at the end of the sample.

Full list: download `Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (22,516 rows, 1.4 MB) from [releases/latest](https://github.com/agentpopulation/22k-indonesia-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

Excel users: Data > From Text/CSV, UTF-8. Files are UTF-8 without a byte-order mark and comma-separated.

## Columns and tags

<details>
<summary>Columns, types and tags</summary>

| Column | Type | Example | Meaning |
|---|---|---|---|
| url | string | [https://data.lamongankab.go.id/dataset/…](https://data.lamongankab.go.id/dataset/000530db-f7eb-4dc3-a187-ad77f6f025af/resource/1d59eceb-5db9-4033-9bd3-4f09ff4ce3e9/download/data_statistik.json) | The address that was tested |
| title | string | Bantuan Hukum - Periode Juni 2023 - Dat… | Station, dataset or feed name |
| service | string | Portal Data Lamongan | The service the endpoint belongs to; joins to the services file together with host |
| host | string | data.lamongankab.go.id | Host name of the address |
| country | string | ID | ISO 3166-1 alpha-2 code, or EU; empty when global or unknown |
| category | string | Statistics & Economy | Category of the endpoint |
| subcategory | string |  | Left empty from the 15 Nov 2026 snapshot; kept so the columns stay the same |
| format | string | json | What the test call returned: json, csv, geojson, xml, gtfs, zip, txt and so on |
| tags | string | `no-key\|json\|agent-ready` | Tags separated by \| |
| last_tested | date | 2026-11-16 | Date of the test call, YYYY-MM-DD (IST) |

| Tag | Rows | Meaning |
|---|---:|---|
| agent-ready | 22,516 | No key sent, JSON body, passed a data call on last_tested |
| json | 22,516 | Format of the body |
| no-key | 22,516 | No key was sent in the test call |

A machine-readable copy of this dictionary is in [datapackage.json](datapackage.json).

</details>

## Known limits

- 924 rows are map-layer queries with resultRecordCount set: the tested call asked for a few records; change the query to get the full layer.
- 921 rows are layers on ArcGIS Online, where anyone can publish: some are class projects, tests or copies. Check the owner and the fields before you rely on one. Layers whose titles read as a test, draft or copy are not used as starting points; named organisations come first in the recommended lists.
- 72 rows have a title that reads as a test, a draft, a copy or a sample; they are not used as starting points.
- The country code (ID) is the code the endpoint is filed under, not the place the data covers and not always the publisher's country. Where a row had no code, the code of its ArcGIS organisation is used when that organisation lists one country only. In a sample of 14 titles read before release, none was about a place outside Indonesia. Most rows come from one regency portal (Lamongan), which lists each table as JSON and as CSV; this pack holds the JSON rows only. Filter by title or service if you need data about one place.
- Stations and feeds can go quiet after their test date; re-test a URL before you rely on it.
- Not in this pack: endpoints that need a key or a POST, and URLs that did not pass.
- Left out: 13 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 4 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 21 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 1 row that is another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 63 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 6 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 284 rows of university, college and school organisations and hosts (many of their layers are students' work).
- Left out: 667 rows that are another address form of an ArcGIS layer already in an earlier pack of the collection (the same rows under another query).
- Left out: 49 rows that are a second address form of an ArcGIS layer in this list (the same rows under another query); one address is kept per layer, the newest test first.

## Licence and credit

> [!IMPORTANT]
> This list (URLs, titles, tags and test results) is © 2026 AgentPopulation, released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit AgentPopulation and link agentpopulation.com. The data each endpoint returns belongs to its provider and stays under that provider's terms; this licence does not cover it.

Copy-ready credit:

`Indonesia API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.`

GitHub's "Cite this repository" button reads [CITATION.cff](CITATION.cff).

<!-- agentpopulation:start -->
## Part of 10M API endpoints for AI agents

This pack is one of the 50 topic packs of [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents), the open collection by [AgentPopulation](https://agentpopulation.com). Target: 10 million+ open API endpoints that pass a keyless API call.

AgentPopulation's test run of 16 Nov 2026: 4,452,803 tested, 3,346,053 passed a data call. This is the Indonesia pack: 22,516 endpoints from 59 services, none of them in a pack read from the earlier snapshot, by address or as another address of the same map layer. Packs overlap, so an endpoint can appear in more than one.

For the latest tested endpoints, search [agentpopulation.com/apis](https://agentpopulation.com/apis). This pack is a snapshot from 16 Nov 2026.

Sibling packs that share the most URLs with this one: [59k-europe-region-arcgis-apis-for-agents](https://github.com/agentpopulation/59k-europe-region-arcgis-apis-for-agents) (10 shared) · [25k-arcgis-server-apis-for-agents](https://github.com/agentpopulation/25k-arcgis-server-apis-for-agents) (3 shared). The rest are listed in [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents).

Questions, pack requests, reports of endpoints that stopped answering and requests to remove a row go to [Discussions](https://github.com/agentpopulation/10m-open-apis-for-ai-agents/discussions), or to [@agentpopulation](https://x.com/agentpopulation) on X. The packs are a work in progress and corrections are welcome.

Spotted a wrong row or a dead URL? Tell us on X: [@agentpopulation](https://x.com/agentpopulation).

If this pack saved you time, a star helps others find it.

---

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents)

<!-- agentpopulation:end -->
