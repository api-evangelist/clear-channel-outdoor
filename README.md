# Clear Channel Outdoor (clear-channel-outdoor)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
