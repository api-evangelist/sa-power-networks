# SA Power Networks (sa-power-networks)

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

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
