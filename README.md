# Universiti Teknologi Malaysia (utm)

Universiti Teknologi Malaysia (UTM) is a public research university in Johor Bahru and Kuala Lumpur, Malaysia, ranked #181 in the QS World University Rankings 2025. This repository catalogs UTM's public developer and API footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/utm/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=utm-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Access, Institutional Repository, OAI-PMH, Malaysia

## APIs

- **UTM Institutional Repository (UTM-IR) OAI-PMH** — EPrints-based OAI-PMH 2.0 metadata harvesting endpoint for UTM research output (theses, articles, conference papers). Base URL: `http://eprints.utm.my/cgi/oai2`. Docs: [UTM Library](https://library.utm.my/utm-institutional-repository/), [Sherpa registry](https://v2.sherpa.ac.uk/id/repository/987). Documented by open-access registries; not verified live from the cataloging environment.

UTM does not publish a dedicated public developer portal or documented REST APIs. The OAI-PMH repository feed is the only machine-consumable public interface confirmed via registries.

## Plans, Rate Limits & FinOps

- [Plans / Pricing](plans/utm-plans-pricing.yml)
- [Rate Limits](rate-limits/utm-rate-limits.yml)
- [FinOps](finops/utm-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://www.utm.my/
- Library: https://library.utm.my/
- Developer/Digital Portal: https://digital.utm.my/
- Authentication (myUTM SSO): https://my.utm.my/login
- LinkedIn: https://www.linkedin.com/school/universiti-teknologi-malaysia/

## Notes

All listed properties were probed during cataloging. The main portal, library, UTMDigital, and myUTM login returned HTTP 200. The UTM-IR OAI-PMH endpoint (`http://eprints.utm.my/cgi/oai2`) is documented by ROAR, OpenDOAR, and Sherpa but did not resolve from the cataloging environment, so its live status is recorded as unverified (0). No official UTM GitHub organization was found, and no endpoints were fabricated. See [review.yml](review.yml) for per-URL verification details.

## Maintainers

- Kin Lane — kin@apievangelist.com
