# City University of Hong Kong (cityu)

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

City University of Hong Kong (CityUHK) is a publicly funded (UGC) research university in Kowloon, Hong Kong SAR. This repository catalogs the institution's public developer and API footprint as an [APIs.json](https://apisjson.org/) profile. CityUHK's openly machine-readable surface is small and, with one exception, TENANTED rather than built: CityUHK Scholars is an Elsevier Pure deployment (scholars.cityu.edu.hk is a CNAME to cityu.elsevierpure.com), Canvas is an Instructure tenant, and single sign-on runs on an Okta tenant at auth.cityu.edu.hk. The exception, and the one machine-readable contract CityUHK operates itself, is its Shibboleth Identity Provider at idp2.cityu.edu.hk, registered in eduGAIN through the Hong Kong Access Federation.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=cityu-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Hong Kong, China, Research, Institutional Repository, OAI-PMH, Identity Federation, Research Data, Learning Management

## APIs

Every surface carries an operator: `institution` means CityUHK runs the thing the contract describes; `tenant` means CityUHK's account on a vendor platform, where the data is CityUHK's and the contract is not.

- **CityUHK Shibboleth Identity Provider** — `institution` — CityUHK's own SAML 2.0 IdP, publishing live Shibboleth metadata and registered in eduGAIN via the Hong Kong Access Federation. Metadata: https://idp2.cityu.edu.hk/idp/shibboleth
- **CityUHK Scholars OAI-PMH** — `tenant` — Public OAI-PMH 2.0 endpoint for the CityUHK Scholars repository. Open, no authentication. Base: https://scholars.cityu.edu.hk/ws/oai
- **CityUHK Scholars Pure Web Service** — `tenant` — CityUHK's deployment of the Elsevier Pure REST web service at https://scholars.cityu.edu.hk/ws/api, gated by an api-key header. The contract is Elsevier's Pure API 5.35.1-2, a generic product specification, and is deliberately not stored here.
- **CityUHK Single Sign-On (OIDC / OAuth 2.0)** — `tenant` — Okta authorization server on CityUHK's own hostname, serving public OIDC Discovery and RFC 8414 metadata. Issuer: https://auth.cityu.edu.hk
- **CityUHK Canvas LMS** — `tenant` — Instructure tenant at canvas.cityu.edu.hk, SSO-gated. No CityUHK LTI registration is publicly readable.

## Plans / Rate Limits / FinOps

- Plans: [plans/cityu-plans-pricing.yml](plans/cityu-plans-pricing.yml)
- Rate Limits: [rate-limits/cityu-rate-limits.yml](rate-limits/cityu-rate-limits.yml)
- FinOps: [finops/cityu-finops.yml](finops/cityu-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.cityu.edu.hk/
- GitHub: https://github.com/cityu (official org; no public repositories)
- LinkedIn: https://hk.linkedin.com/school/cityu/
- Research Repository: https://scholars.cityu.edu.hk/
- Identity Federation: https://idp2.cityu.edu.hk/idp/shibboleth
- AI Policy: https://www.cityu.edu.hk/GenAI/guidelines.htm
- AI Tooling: https://www.cityu.edu.hk/GenAI/gpt-services.htm
- API Programme (internal, MuleSoft Anypoint): https://www.cityu.edu.hk/its/services-facilities/api-gateway-and-api-management
- Authentication: [authentication/cityu-authentication.yml](authentication/cityu-authentication.yml)
- Standards Conformance: [conformance/cityu-education-standards-conformance.yml](conformance/cityu-education-standards-conformance.yml)
- Review: [review.yml](review.yml)

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles who OPERATES a
surface before saving any contract.

The 34 OpenAPI definitions this repository previously held were not CityUHK's. Each carried
`info.title: "Pure <resource> API"`, `info.contact.email: pure-support@elsevier.com` and
`servers: ["/ws/api"]` — Elsevier's generic Pure API 5.35.1-2 product contract, shipped identically
by at least nine other institutions in the cohort, split into 34 per-tag documents by our own refine
step and then into 34 `apis[]` entries. DNS confirms it independently: `scholars.cityu.edu.hk` is a
CNAME to `cityu.elsevierpure.com`. Those 34 specs and the 84 collections, JSON Schemas, JSON
Structures, examples, Spectral rules, vocabularies, JSON-LD contexts, capability edges and
agentic-access files derived from them — 118 files — were removed. The Pure deployment is now
recorded once, as a tenant relationship.

Newly found and verified in the same pass: CityUHK operates its own Shibboleth Identity Provider at
`idp2.cityu.edu.hk`, publishing live SAML 2.0 IdP metadata and registered in eduGAIN through the
Hong Kong Access Federation; the OAI-PMH endpoint is genuinely open and rich (persons, publications,
student theses, datasets, an OpenAIRE set, with ORCID iDs inline in the harvested Dublin Core); and
single sign-on runs an Okta authorization server on CityUHK's own hostname with public OIDC
Discovery and RFC 8414 metadata.

CityUHK's IT Services does run a real API gateway and API management practice on MuleSoft Anypoint,
used to connect campus systems, but none of that catalogue is published or callable off-campus and
there is no developer portal. No open-data portal, course/timetable/SIS API, or status page was
found; `data.cityu.edu.hk` and `opendata.cityu.edu.hk` do not resolve. The entire
`www.cityu.edu.hk` estate is served behind an Imperva/Incapsula bot challenge that returns HTTP 200
with a challenge body on every deep path, so pointers into it are recorded as live-but-unreadable.

No endpoints were fabricated. The corrected footprint is one institution-operated machine-readable
contract and four tenant surfaces, which is a lower score than the 34-spec profile it replaces.

## Maintainers

- Kin Lane — kin@apievangelist.com
