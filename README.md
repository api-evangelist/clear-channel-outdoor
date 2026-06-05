# Clear Channel Outdoor (clear-channel-outdoor)

Clear Channel Outdoor (NYSE: CCO) is one of the largest out-of-home (OOH) advertising companies in the world, operating billboards, street furniture, transit, airport, and digital out-of-home (DOOH) displays across 65+ U.S. markets and 55+ commercial airports, reaching "130 million Americans weekly." The CCO developer surface spans three layers: the CCO.IO Automated Direct REST API at direct.cco.io for programmatic-direct buying of inventory (OAuth 2.0 client credentials, open-source Go SDK at github.com/ClearChannelOutdoor/io-sdk-golang), programmatic digital out-of-home (pDOOH) buying through 20+ DSP partners using OpenRTB 2.6 with the DOOH object extension, and RADAR — CCO's first-party audience and attribution data suite (RADARView, RADARProof, RADARConnect, RADARSync, Inflight Insights) built on aggregated and anonymous mobile location data. CCO maintains a public fork of the IAB Tech Lab OpenDirect-OOH specification at github.com/ClearChannelOutdoor/ooh_open_direct.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/clear-channel-outdoor/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/clear-channel-outdoor/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Advertising
- Out Of Home
- OOH
- Programmatic
- Digital Out Of Home
- DOOH
- pDOOH
- OpenRTB
- OpenDirect
- Billboards
- Transit Advertising
- Airport Advertising
- Audience Measurement
- Location Data

## Timestamps

- **Created:** 2026-05-22
- **Modified:** 2026-05-23

## APIs

### Clear Channel Outdoor Automated Direct API

REST API for the CCO.IO Automated Direct platform at direct.cco.io. Supports search, retrieval and management of displays, networks, markets, products, orders, bookings, campaigns, creatives, photos, customers, accounts, contracts, quotes, renewals, restrictions and IAB / OpenOOH taxonomies. Uses OAuth 2.0 client credentials (tokenUrl https://direct.cco.io/v2/token) with scoped access tokens. The OpenAPI documented here is derived from the open-source Go SDK at github.com/ClearChannelOutdoor/io-sdk-golang and from the developer portal at developer.cco.io.

- **Human URL:** [https://developer.cco.io](https://developer.cco.io)
- **Base URL:** `https://direct.cco.io`

#### Tags

- Programmatic Direct
- DOOH
- OOH
- REST
- OAuth2

#### Properties

- [Documentation](https://developer.cco.io)
- [OpenAPI](openapi/clear-channel-outdoor-direct-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [SDK](https://github.com/ClearChannelOutdoor/io-sdk-golang)
- [Authentication](https://direct.cco.io/v2/token)
- [Spectral Rules](rules/clear-channel-outdoor-direct-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

### Clear Channel Outdoor pDOOH RTB Supply

Programmatic digital out-of-home (pDOOH) supply made available through 20+ DSP partners that transact CCO inventory via OpenRTB 2.6 with the DOOH object extension (with imp.qty support and the OpenOOH venue taxonomy where venuetypetax=1). This is not a CCO- hosted REST API — it is a supply-chain contract that buyers access through DSPs/SSPs (Vistar Media, Hivestack, The Trade Desk, Google DV360, etc.). Documented here so the contract, partners and schemas are first-class artifacts in the network.

- **Human URL:** [https://clearchanneloutdoor.com/programmatic-advertising/](https://clearchanneloutdoor.com/programmatic-advertising/)

#### Tags

- pDOOH
- OpenRTB
- DSP
- SSP
- RTB

#### Properties

- [Documentation](https://clearchanneloutdoor.com/programmatic-advertising/)
- [Standards](https://github.com/InteractiveAdvertisingBureau/openrtb2.x)
- [JSON Schema](json-schema/clear-channel-outdoor-openrtb-dooh-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/clear-channel-outdoor-dsp-integration-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Examples](examples/clear-channel-outdoor-openrtb-dooh-bid-request-example.json)

### Clear Channel Outdoor RADAR Data Suite

RADAR is CCO's first-party audience-planning, attribution and measurement suite built on aggregated and/or anonymous mobile location data licensed from business partners. The suite includes RADARView (planning), RADARProof (attribution), RADARConnect (audience activation), RADARSync (data sync), and Inflight Insights — described as "the first in-house measurement solution offered by an OOH media owner to deliver visitation analytics during a campaign flight." RADAR is delivered as a managed data/services offering; there is no public self-serve API. Documented here so the product family, scope and data semantics are catalogued in the network.

- **Human URL:** [https://clearchanneloutdoor.com/radar-data-solutions/](https://clearchanneloutdoor.com/radar-data-solutions/)

#### Tags

- Audience Data
- Attribution
- Location Data
- Measurement
- Planning

#### Properties

- [Documentation](https://clearchanneloutdoor.com/radar-data-solutions/)
- [Privacy](https://clearchanneloutdoor.com/privacy-policy/)

## Common Properties

- [Website](https://clearchanneloutdoor.com)
- [Developer Portal](https://developer.cco.io)
- [Portal](https://developer.cco.io)
- [Programmatic Advertising](https://clearchanneloutdoor.com/programmatic-advertising/)
- [Data Solutions](https://clearchanneloutdoor.com/radar-data-solutions/)
- [Git Hub](https://github.com/ClearChannelOutdoor)
- [GitHub Organization](https://github.com/ClearChannelOutdoor)
- [LinkedIn](https://www.linkedin.com/company/clear-channel-outdoor)
- [Investor Relations](https://investor.clearchannel.com)
- [Privacy Policy](https://clearchanneloutdoor.com/privacy-policy/)
- [JSON-LD](json-ld/clear-channel-outdoor-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/clear-channel-outdoor-vocabulary.yml)
- [Plans](plans/clear-channel-outdoor-plans-pricing.yml)
- [Rate Limits](rate-limits/clear-channel-outdoor-rate-limits.yml)
- [Fin Ops](finops/clear-channel-outdoor-finops.yml)
- [SDK](https://github.com/ClearChannelOutdoor/io-sdk-golang)
- [Standards](https://github.com/ClearChannelOutdoor/ooh_open_direct)
- [Products](https://clearchanneloutdoor.com)
- [Integrations](https://clearchanneloutdoor.com/programmatic-advertising/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
