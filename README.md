# City University of Hong Kong (cityu)

City University of Hong Kong (CityUHK) is a publicly funded research university in Kowloon, Hong Kong SAR, ranked #55 in the QS World University Rankings 2025. This repository catalogs the institution's public developer and API footprint as an [APIs.json](https://apisjson.org/) profile. CityUHK's openly machine-readable surface is modest, centered on its research information system, CityUHK Scholars (Elsevier Pure), which exposes a public OAI-PMH metadata endpoint.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=cityu-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Institutional Repository, OAI-PMH, Hong Kong, China

## APIs

- **CityUHK Scholars OAI-PMH** — Public OAI-PMH 2.0 endpoint for the CityUHK Scholars institutional repository / research information system. Docs: https://scholars.cityu.edu.hk/ — Base: https://scholars.cityu.edu.hk/ws/oai
- **CityUHK Scholars Pure Web Service (REST)** — Elsevier Pure OpenAPI 3 CRUD REST service backing CityUHK Scholars; gated, requires an API key (returns HTTP 401 without credentials). Docs: https://scholars.cityu.edu.hk/

## Plans / Rate Limits / FinOps

- Plans: [plans/cityu-plans-pricing.yml](plans/cityu-plans-pricing.yml)
- Rate Limits: [rate-limits/cityu-rate-limits.yml](rate-limits/cityu-rate-limits.yml)
- FinOps: [finops/cityu-finops.yml](finops/cityu-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.cityu.edu.hk/
- GitHub: https://github.com/cityu (official org; no public repositories)
- LinkedIn: https://hk.linkedin.com/school/cityu/
- Developer Portal: https://scholars.cityu.edu.hk/
- Review: [review.yml](review.yml)

## Notes

All entries were verified against live URLs in June 2026; no endpoints were fabricated. The CityUHK Scholars OAI-PMH endpoint was confirmed live (HTTP 200, `verb=Identify` returns repository "CityUHK Scholars", protocol 2.0). The Pure REST Web Service is OpenAPI 3-described but gated (HTTP 401 without an API key) and is listed for completeness. The official GitHub organization exists but currently publishes no public repositories. No public open-data portal, course/timetable/SIS API, or status page was confirmed for the institution; core systems (AIMS, CAP, Canvas, CityUHK Portal) are authenticated and not publicly documented as APIs.

## Maintainers

- Kin Lane — kin@apievangelist.com
