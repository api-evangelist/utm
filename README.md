# Universiti Teknologi Malaysia (utm)

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
