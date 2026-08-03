# Arbol

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

Arbol is a global climate risk solutions platform providing parametric and traditional insurance and weather derivatives. Founded in 2018 and headquartered in New York, Arbol combines AI/ML-driven underwriting, institutional-grade climate data sourced from NOAA, NASA and ESA, and dedicated risk capital to close the global insurance protection gap. Coverage spans agriculture, energy, travel, wildfire and reinsurance, with parametric products that pay out on objective weather triggers rather than loss adjustment.

Its licensed underwriting arm, Arbol Insurance Services (AIS), holds binding authority from an A.M. Best "A" rated carrier and Lloyd's coverholder status, and distributes named storm, precipitation, temperature, wind, snow, solar and soil-moisture products through licensed producers across all 50 U.S. states. Arbol Insurance Services UK Ltd is an FCA-regulated MGA serving the rest of the world through the Lloyd's global licensing network.

## API surface

**Arbol publishes no public developer API.** Quoting, binding and policy issuance are delivered through the broker/agent web platform at `app.arbol.io`, which is credentialed and closed to licensed producers. Contract discovery was run in full on 2026-08-02 across every public host — REST OpenAPI on API/docs host roots, GraphQL introspection, MCP `tools/list`, A2A agent cards and the `/.well-known/` surface — and every probe missed. See [`contract-discovery.yml`](contract-discovery.yml) for the recorded evidence.

## What is captured here

| Artifact | What it holds |
|---|---|
| [`llms/`](llms/) | Three verbatim `llms.txt` files Arbol serves from `www.arbol.io`, `insurance.arbol.io` and `insurance.arbol.uk` |
| [`packages/`](packages/) | Registry sweep; one legacy first-party PyPI package (`dweather-client`, 2021) and the public GitHub org |
| [`well-known/`](well-known/) | Full `/.well-known/` sweep across four hosts — recorded negative result |
| [`conformance/`](conformance/) | Insurance regulatory posture (state licensure, A.M. Best, Lloyd's, FCA) and GDPR/UK GDPR; no API standards assertable |
| [`security/`](security/) | Probed TLS/HSTS/DNSSEC/CAA/SPF/DMARC posture for the Arbol hosts and domains |
| [`contract-discovery.yml`](contract-discovery.yml) | The full record of what was probed and what missed |

- Website: https://www.arbol.io/
- Insurance Services (US): https://insurance.arbol.io/
- Insurance Services (UK): https://insurance.arbol.uk/
- Platform: https://app.arbol.io/
- GitHub: https://github.com/Arbol-Project
