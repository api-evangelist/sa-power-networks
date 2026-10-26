# SA Power Networks (sa-power-networks)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

SA Power Networks is South Australia's sole electricity distributor — the poles-and-wires DNSP that builds, maintains and upgrades the network delivering power to around 900,000 homes and businesses, and the operator of the state's Flexible Exports dynamic solar export scheme. It sits between the transmission network and the retailers, holding meter data, network capacity data and DER connection data but selling nothing to consumers directly. Its API posture is empty by design: Australia's Consumer Data Right was extended to energy and is live, but the designation names electricity retailers as primary data holders and AEMO as the secondary data holder — distributors are not designated, and SA Power Networks does not appear among the 84 brands on the live CDR energy register. There is no developer portal, no documented API, and no machine-readable contract of any kind. Third parties reach a customer's meter data only by registering as an Authorised Representative and logging into a web portal; network capacity is a registration-gated map viewer; the genuinely open surface is bulk file downloads (zone substation data, the Distribution Annual Planning Report, the embedded generation register) that anyone can pull anonymously but that carry a redistribution restriction rather than an open licence.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sa-power-networks/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sa-power-networks/refs/heads/main/apis.yml)

## Tags

- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Smart Metering
- Solar
- DER
- Open Data

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-07-27

## APIs

No public, documented APIs were found.

Every developer-facing probe returned nothing. The subdomains `developer.`, `developers.`, `docs.`, `api.`, `apis.`, `data.`, `open.` and `opendata.sapowernetworks.com.au` do not resolve (NXDOMAIN). On the main site, `/developers`, `/developer`, `/api`, `/apis`, `/docs`, `/data`, `/open-data`, `/openapi.json`, `/swagger.json`, `/api-docs`, `/.well-known/openid-configuration` and `/.well-known/security.txt` all return HTTP 404. The published `sitemap.xml` (547 URLs) contains zero matches for `cdr`, `consumer-data`, `open-data`, `/api` or `green-button`; the only five hits on "developer" are property-developer connection pages.

See `review.yml` for the full mandate, standard, access-gate and auth findings.

## Mandate Posture

- **Regime in the home market:** Consumer Data Right (Energy) — live, statutory, ACCC-administered, Data Standards Body-specified.
- **Status for this organization:** not applicable. Distributors are not designated data holders. Verified against the live CDR Register — `https://api.cdr.gov.au/cdr-register/v1/energy/data-holders/brands/summary` returned HTTP 200 with 84 energy brands, every one a retailer, and no distribution network service provider of any kind.
- **The obligation that does bite:** the South Australian Government's Dynamic Export Limits requirement (in force 1 July 2023), which makes new solar installations dynamic-exports capable and puts SA Power Networks in the role of dispatching export limits. That obligation is implemented and live for customers — and it is the one place SA Power Networks operates something API-shaped — but no endpoint, specification, or standard reference for it is published anywhere by SA Power Networks.

## Common Properties

- [Website](https://www.sapowernetworks.com.au/)
- [LinkedIn](https://www.linkedin.com/company/sa-power-networks)
- [About](https://www.sapowernetworks.com.au/about-us/our-role/)
- [Industry](https://www.sapowernetworks.com.au/industry/)
- [Blog](https://www.sapowernetworks.com.au/industry/industry-news/)
- [Resource Library](https://www.sapowernetworks.com.au/resource-library/)
- [Portal](https://dapr.sapowernetworks.com.au/)
- [Documentation](https://www.sapowernetworks.com.au/industry/access-your-clients-meter-data/)
- [Documentation](https://www.sapowernetworks.com.au/industry/flexible-exports/)
- [Documentation](https://www.sapowernetworks.com.au/industry/relevant-agent/)
- [Data](https://www.sapowernetworks.com.au/industry/annual-network-plans/)
- [Data](https://www.sapowernetworks.com.au/data/324688/2024-2025-zone-substation-data/)
- [Portal — Industry Portal](https://www.sapowernetworks.com.au/industry/portal/)
- [Support](https://www.sapowernetworks.com.au/contact-us/)
- [Privacy Policy](https://www.sapowernetworks.com.au/policies/privacy-policy/)
- [Terms of Service — website disclaimer](https://www.sapowernetworks.com.au/policies/disclaimer/)

## Artifacts

Enrichment round 2026-07-27. Every artifact below records what was actually probed, including the negatives.

- `well-known/sa-power-networks-well-known.yml` — `/.well-known/` probe matrix across four hosts. One document exists.
- `well-known/sa-power-networks-meterdata-openid-configuration.json` — verbatim OIDC discovery document from the Your Meter Data portal (HTTP 200), plus its JWKS.
- `authentication/sa-power-networks-authentication.yml` — both portal auth surfaces (Salesforce Experience Cloud OIDC, AWS Cognito implicit) and what is absent.
- `scopes/sa-power-networks-scopes.yml` — the OIDC `scopes_supported` set, flagged as Salesforce platform defaults rather than an SA Power Networks authorization model.
- `conformance/sa-power-networks-conformance.yml` — IEEE 2030.5 / CSIP-AUS conformance with evidence from SA Power Networks' own trial reports; CDR, OpenAPI, security.txt and api-catalog all recorded as non-conforming.
- `lifecycle/sa-power-networks-lifecycle.yml` — no API versioning, deprecation policy, SLA or status page; the outage map is network status, not API status.
- `llms/sa-power-networks-llms.txt` — generated (the provider serves no `/llms.txt`).
- `security/sa-power-networks-domain-security.yml` — probed TLS/HSTS/DNSSEC/CAA/SPF/DMARC.

Two round-one findings were corrected this round (see the `correction:` blocks in `review.yml`): SA Power Networks **does** name IEEE 2030.5 and CSIP-AUS in its own published Flexible Exports Lessons Learnt reports, and an OpenID Connect discovery document **is** reachable — on the meter-data portal, not on the Cognito domain. Neither changes the headline: still no API.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
