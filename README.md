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

Universiti Teknologi Malaysia (UTM) is a public research university in Johor Bahru and Kuala Lumpur, Malaysia — one of the five institutions designated a Research University by the Ministry of Higher Education, and ranked #181 in the QS World University Rankings 2025. This repository catalogs UTM's public programmable footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/utm/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=utm-api-evangelist&utm_content=repo

## Type

- **Class:** university (`x-type: university`)
- **Category:** Public Research University
- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

University, Higher Education, Education, Public Research University, Technical University, Malaysia, Research, Open Access, Institutional Repository, Research Repository, Scholarly Publishing, OAI-PMH, Identity Federation, SAML, Crossref

## Who operates what

A university is a federation of buyers, not a producer, so every surface below carries an `x-operator` saying **who runs the thing it describes** — which is rarely the same answer as who the domain belongs to. Operator was settled by IP ownership as well as hostname: `whois` on **161.139.0.0/16** returns netname **UTM-MY**, "Universiti Teknologi Malaysia", country MY, and every UTM host named here sits inside it.

| Surface | `x-operator` | Status |
|---|---|---|
| UTMIK Repository (DSpace-CRIS) — OAI-PMH + REST | `institution` | OAI-PMH 200, REST root 200, collections 403 |
| UTM Press Journals (Open Journal Systems) — OAI-PMH | `institution` | OAI-PMH 200, REST API v1 401 |
| UTM Microsoft Entra ID tenant — SAML 2.0 / OpenID Connect | `federation` | 200, signed metadata |
| Crossref membership — Penerbit UTM Press, member 4787 | `registry` | 200 |
| ROR registration — `ror.org/026w31v75` | `registry` | 200 |
| UTM-IR EPrints (`eprints.utm.my`) | `institution` | unreachable — connection refused |

No vendor contract is saved in this repository. The repository and journal software (DSpace-CRIS, PKP Open Journal Systems) belongs to those projects; what belongs to UTM is the deployment, the host, the content and the administrative contact, and that is what is recorded.

## APIs

- **UTMIK Repository (DSpace-CRIS)** — UTM's institutional knowledge repository on `utmik.utm.my`. The OAI-PMH 2.0 endpoint answers anonymously as "UTMIK Repository" (adminEmail `library.automation@utm.my`, earliest record 2025-01-27) in twelve metadata formats — `oai_dc`, `qdc`, `mods`, `mets`, `didl`, `ore`, `rdf`, `marc`, `dim`, `etdms`, `rioxx`, `uketd_dc` — and advertises an OpenAIRE CERIF-for-CRIS 1.1 profile at `/server/oai/openairecris`. Sets include RESEARCH DATA, SCHOLARLY PUBLICATION, UTM ARCHIVE, UTM LENSES and CITIZEN SCIENCE. Base URL: `https://utmik.utm.my/server/oai/request`.
- **UTM Press Journals (OJS)** — `journals.utm.my`, harvestable since 2011-12-12 as "UTM Press Journal Management powered by OJS". The per-journal REST API v1 is live but token-gated. Base URL: `https://journals.utm.my/index/oai`.
- **UTM identity federation** — Microsoft Entra ID tenant `9c827912-3502-4333-ba47-1b242c3d20e6`, bound to UTM by domain ownership (realm discovery on `user@utm.my` returns FederationBrandName "Universiti Teknologi Malaysia"). Signed SAML 2.0 metadata under entityID `https://sts.windows.net/9c827912-3502-4333-ba47-1b242c3d20e6/` plus a full OIDC discovery document. This is the most completely specified machine contract UTM has.
- **Crossref membership** — Penerbit UTM Press is member **4787**, prefix **10.11113**, 12,640 registered DOIs. *Jurnal Teknologi (Sciences & Engineering)* (ISSN 0127-9696 / 2180-3722) carries 6,311 DOIs with deposits in every year from 2011 through 2026.
- **ROR registration** — `https://ror.org/026w31v75`, domain `utm.my`, established 1975, GRID `grid.410877.d`, ISNI `0000 0001 2296 1505`, plus four Crossref Open Funder Registry identifiers recording UTM as a research funder.
- **UTM-IR EPrints** — retained as a documented relationship, not credited as a live surface. See below.

## What UTM does not publish

UTM publishes **no developer portal, no API documentation, and no OpenAPI, AsyncAPI or JSON Schema of its own**, and there is no route by which an unaffiliated developer can obtain a credential for anything it runs. Probed and confirmed absent:

- `www.utm.my` sitemap contains exactly one policy page and no API, developer or open-data page.
- `api.utm.my` resolves and returns HTTP 200 — with a **17-byte empty IIS document** — and 404s on `/swagger`, `/swagger/v1/swagger.json`, `/openapi.json`, `/docs`, `/v1` and `/.well-known/openapi`. A soft-404, not a surface.
- No official UTM GitHub organization. The two name-matching orgs hold zero and one unrelated repository.
- No `llms.txt`, no `.well-known/security.txt`.
- Moodle at `elearning.utm.my` is live but exposes no LTI 1.3 or web-service contract (`/mod/lti/auth.php`, `/.well-known/jwks.json`, `/webservice/rest/server.php` all 404).
- No DataCite membership — `api.datacite.org` returns zero clients for UTM; DOIs are minted through Crossref.
- No Shibboleth IdP under `utm.my`, and no UTM entry in the eduGAIN export (7.8 MB parsed, zero matches). SIFULAN, the Malaysian Access Federation, returned 403 to every probe, so its membership is neither confirmed nor denied.

## Unreachable hosts

- **`eprints.utm.my`** — the legacy EPrints institutional repository, still registered with ROAR (1358), OpenDOAR and Sherpa (987) and still linked from the UTM Library. DNS resolves to `161.139.21.110` on UTM's own allocation, but the host **refused connections on both port 80 and port 443** from this environment and returned HTTP 522 through two independent public proxies. UTMIK, whose earliest record is dated 2025-01-27, appears to be its successor.
- **`utmik.utm.my`** answered fully at **17:26Z on 2026-09-01** — the OAI-PMH `responseDate` is the server's own proof — then stopped answering this environment and two public proxies later the same day. Its pointers may grade dead on a re-probe; the surface is real.
- **`openscience.utm.my`** and **`hpc.utm.my`** resolve but do not connect. No open-science portal or HPC service catalog is claimed.

## Domain standard conformance (Kin Score `education` regime)

Reward-only, read from responses and never from a prose claim — UTM makes no conformance claims anywhere public. See [conformance/utm-conformance.yml](conformance/utm-conformance.yml).

| Standard | Status | Operator |
|---|---|---|
| `oai-pmh` 2.0 | confirmed | institution (two independent endpoints) |
| `crossref` | confirmed | institution (member 4787) |
| `saml` 2.0 | confirmed | federation (Entra ID tenant) |
| `orcid` | partial | institution (DSpace-CRIS ORCID endpoints advertised; records 403) |
| `shibboleth` | not-found | deciding source unreadable, not negative |
| `datacite`, `scim`, `lti`, `oneroster`, `ed-fi`, `caliper`, `qti` | not-found | — |

## Artifacts

- [Conformance](conformance/utm-conformance.yml) — `education` regime domain standards, probed
- [Identity federation](identity-federation/utm-identity-federation.yml) — Entra ID tenant, SAML + OIDC
- [Authentication](authentication/utm-authentication.yml) — auth posture across every reachable surface
- [Plans / Pricing](plans/utm-plans-pricing.yml) · [Rate Limits](rate-limits/utm-rate-limits.yml) · [FinOps](finops/utm-finops.yml) · [Domain Security](security/utm-domain-security.yml)
- [review.yml](review.yml) — per-URL verification, June 2026 and September 2026 passes

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-09-01

## Common Properties

- Website: https://www.utm.my/
- Library: https://library.utm.my/
- Research Repository: https://utmik.utm.my/
- Identity Federation: https://login.microsoftonline.com/utm.my/v2.0/.well-known/openid-configuration
- Single Sign-On (MyUTM): https://my.utm.my/login
- AI Policy: [Guidelines for the Use of Generative AI in Teaching and Learning, UTM](https://fke.utm.my/wp-content/uploads/2024/11/Guidelines-for-the-Use-of-Generative-Artificial-Intelligence-in-Teaching-and-Learning-UTM-1.pdf)
- Blog: https://news.utm.my/
- Privacy Policy: https://www.utm.my/privacy-policy/
- LinkedIn: https://www.linkedin.com/school/universiti-teknologi-malaysia/

## Changes in the 2026-09-01 re-profile

Three institution-operated surfaces the June 2026 pass missed were found and verified: the UTMIK Repository, the UTM Press journal platform, and UTM's identity federation. Two registry memberships were recorded. **One pointer was removed** — the `DeveloperPortal` claim on `https://digital.utm.my/`. That host is live and is a genuine UTM property, but it is the Office of Quality & Digital Transformation (UTMDX), an administrative office site: no API documentation, no keys, no registration. Claiming a developer program UTM does not run is the presence-is-not-provenance error the university pipeline exists to prevent, and removing it lowers this profile's score, which is the correct outcome.

## Maintainers

- Kin Lane — kin@apievangelist.com
