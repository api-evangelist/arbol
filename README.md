# Arbol

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
