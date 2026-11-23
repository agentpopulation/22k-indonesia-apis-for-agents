## Indonesia API endpoints, snapshot 16 Nov 2026

- 22,516 endpoints passed a keyless data call, tested 16 Nov 2026 (IST)
- 59 services · country ID · 22,516 keyless JSON rows

### Download

- `Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz`: the full list, 22,516 rows, 1.4 MB gzipped (8.1 MB as CSV), SHA-256 `662ca4ef802a8dff91ae203da265d034f6bdf18a1b4c30d886260296ff624309`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Indonesia_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 22,516 · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.
- 📱 App features: 22,516 · Show a regency table as a card or a chart, with the period and the source.
- 🧠 Grounding and data pipelines: 22,516 · Load the regency tables on a schedule into your own store, so an agent can cite a dated source.
- 🧪 Evals and testing: 22,516 · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

### Changes

- First release
- Left out: 13 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 4 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 21 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 1 row that is another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 63 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 6 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 284 rows of university, college and school organisations and hosts (many of their layers are students' work).
- Left out: 667 rows that are another address form of an ArcGIS layer already in an earlier pack of the collection (the same rows under another query).
- Left out: 49 rows that are a second address form of an ArcGIS layer in this list (the same rows under another query); one address is kept per layer, the newest test first.
- Overlap: 10 of these URLs are also in 59k-europe-region-arcgis-apis-for-agents.
- Overlap: 3 of these URLs are also in 25k-arcgis-server-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16 Nov 2026; snapshot 16 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 16 Nov 2026.

Credit: Indonesia API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
