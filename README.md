# clear-channel-outdoor

API Evangelist network profile for **Clear Channel Outdoor** (NYSE: CCO) — one of the largest out-of-home (OOH) advertising companies in the world, operating billboards, street furniture, transit, airport, and digital out-of-home (DOOH) displays across 65+ U.S. markets and 55+ commercial airports.

This profile catalogs CCO's three-layer developer / programmatic surface:

1. The **CCO.IO Automated Direct API** at `direct.cco.io` (developer portal at `developer.cco.io`) — programmatic-direct buying of CCO inventory, OAuth 2.0 client credentials, with an open-source Go SDK at [`ClearChannelOutdoor/io-sdk-golang`](https://github.com/ClearChannelOutdoor/io-sdk-golang).
2. The **pDOOH RTB supply chain** — 20+ DSP partners that transact CCO inventory using OpenRTB 2.6 with the DOOH object extension and the OpenOOH venue taxonomy (`venuetypetax=1`).
3. **RADAR** — CCO's first-party audience-planning, attribution, and measurement suite built on aggregated and anonymous mobile location data.

## Artifacts

| Artifact | Path |
|---|---|
| `apis.yml` | [`apis.yml`](apis.yml) |
| OpenAPI — Automated Direct | [`openapi/clear-channel-outdoor-direct-openapi.yml`](openapi/clear-channel-outdoor-direct-openapi.yml) |
| JSON Schema — DOOH Display | [`json-schema/clear-channel-outdoor-display-schema.json`](json-schema/clear-channel-outdoor-display-schema.json) |
| JSON Schema — DSP Integration | [`json-schema/clear-channel-outdoor-dsp-integration-schema.json`](json-schema/clear-channel-outdoor-dsp-integration-schema.json) |
| JSON Schema — OOH Order (OpenDirect) | [`json-schema/clear-channel-outdoor-order-schema.json`](json-schema/clear-channel-outdoor-order-schema.json) |
| JSON Schema — OpenRTB DOOH | [`json-schema/clear-channel-outdoor-openrtb-dooh-schema.json`](json-schema/clear-channel-outdoor-openrtb-dooh-schema.json) |
| JSON Structure — pDOOH supply chain | [`json-structure/clear-channel-outdoor-pdooh-supply-chain-structure.json`](json-structure/clear-channel-outdoor-pdooh-supply-chain-structure.json) |
| JSON-LD context | [`json-ld/clear-channel-outdoor-context.jsonld`](json-ld/clear-channel-outdoor-context.jsonld) |
| Examples | [`examples/`](examples/) |
| Spectral rules | [`rules/clear-channel-outdoor-direct-rules.yml`](rules/clear-channel-outdoor-direct-rules.yml) |
| Naftiko capability — programmatic-direct buying | [`capabilities/programmatic-direct-ooh-buying.yaml`](capabilities/programmatic-direct-ooh-buying.yaml) |
| Naftiko capability — pDOOH RTB supply | [`capabilities/pdooh-rtb-supply.yaml`](capabilities/pdooh-rtb-supply.yaml) |
| Vocabulary | [`vocabulary/clear-channel-outdoor-vocabulary.yml`](vocabulary/clear-channel-outdoor-vocabulary.yml) |
| Plans (pricing) | [`plans/clear-channel-outdoor-plans-pricing.yml`](plans/clear-channel-outdoor-plans-pricing.yml) |
| Rate limits | [`rate-limits/clear-channel-outdoor-rate-limits.yml`](rate-limits/clear-channel-outdoor-rate-limits.yml) |
| FinOps | [`finops/clear-channel-outdoor-finops.yml`](finops/clear-channel-outdoor-finops.yml) |

## CCO.IO Automated Direct API

REST API for buying CCO inventory programmatically. Authentication is OAuth 2.0 client credentials at `https://direct.cco.io/v2/token`. Path families surfaced in the OpenAPI:

`/v1/displays`, `/v1/networks`, `/v1/networks/{id}/displays`, `/v1/markets`, `/v1/products`, `/v1/orders`, `/v1/bookings`, `/v1/campaigns`, `/v1/creatives`, `/v2/creatives`, `/v1/photos`, `/v1/customers`, `/v1/accounts`, `/v1/contracts`, `/v1/quotes`, `/v1/quotes/current`, `/v1/relationships`, `/v1/restrictions`, `/v1/codes`, `/v1/taxa`, `/v2/taxa`, `/v3/taxa`.

These were derived from the open-source Go SDK [`ClearChannelOutdoor/io-sdk-golang`](https://github.com/ClearChannelOutdoor/io-sdk-golang) and the developer portal at [developer.cco.io](https://developer.cco.io).

## pDOOH DSP Partners

CCO supports programmatic DOOH buying through 20+ DSP partners using OpenRTB 2.6 with the DOOH object: Adelphic, Adform, Adomni, AdQuick, Campsite, Displayce, Google DV360, Hivestack, Nexxen, OneView, OutMoove, Pulsepoint, Quotient, Simplifi, Sito, StackAdapt, The Trade Desk, Vistar Media, Xandr, Yahoo, and Zeta.

## RADAR Data Suite

RADAR uses "aggregated and/or anonymous mobile location data in a privacy-conscious manner" to support planning, amplification, and measurement of OOH campaigns. Product family: **RADARView**, **RADARProof**, **RADARConnect**, **RADARSync**, and **Inflight Insights** — described as "the first in-house measurement solution offered by an OOH media owner to deliver visitation analytics during a campaign flight." Delivered as a managed offering rather than a self-serve API.

## Standards

- [OpenRTB 2.6 with DOOH extension](https://github.com/InteractiveAdvertisingBureau/openrtb2.x)
- [OpenDirect-OOH](https://github.com/Outsmart-OOH/ooh_open_direct) (CCO maintains a fork at [`ClearChannelOutdoor/ooh_open_direct`](https://github.com/ClearChannelOutdoor/ooh_open_direct))
- OpenOOH Venue Taxonomy (`venuetypetax=1`)

## Scale

- "130 million Americans reached weekly" (clearchanneloutdoor.com)
- 65+ U.S. markets
- 55+ commercial airports
- ~310,000 displays globally (industry-reported)
- Listed on NYSE as **CCO**

## Notable Absences

- The `developer.cco.io` portal does not publish a hosted OpenAPI spec — the spec in this repo is derived from the open-source Go SDK and portal documentation.
- No public pricing for the Automated Direct API — gated by buyer/agency credentials.
- No public RSS / changelog feed for the developer platform.
- No public status page surfaced.

## Maintainer

[Kin Lane](https://apievangelist.com), API Evangelist — kin@apievangelist.com
