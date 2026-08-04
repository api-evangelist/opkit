# Opkit (opkit)

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

Opkit was a healthcare automation company that built an automated health insurance verification platform purpose-built for telehealth companies and virtual medical practices. The Opkit REST API let engineering teams run insurance eligibility checks, read benefits, look up payers, manage patients, and receive webhook events programmatically. Opkit (YC S21) later pivoted to a generative-AI healthcare call center and was acqui-hired by 11x in late 2024, after which the platform was wound down. This catalog documents the API as it was publicly described while it was operating.

> Status note: As of this catalog's date the Opkit platform appears decommissioned — `www.opkit.co` and `docs.opkit.co` no longer respond and `api.opkit.co` no longer resolves. See [review.yml](review.yml) for details.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/apis.yml)

## Tags

- Healthcare
- Insurance
- Eligibility
- Benefits
- Verification
- Telehealth

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Opkit Eligibility Inquiries API

Create and retrieve real-time insurance eligibility inquiries to determine whether a patient's coverage is active, in- or out-of-network, and what cost-sharing applies. Submitted against a payer for a patient and resolved asynchronously, with results delivered on the inquiry object and via webhooks.

- **Human URL:** [https://docs.opkit.co](https://docs.opkit.co)
- **Base URL:** `https://api.opkit.co/v1`

#### Tags

- Eligibility
- Insurance
- Verification

#### Properties

- [Documentation](https://docs.opkit.co)
- [OpenAPI](openapi/opkit-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opkit.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opkit.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Opkit Benefits API

Read structured benefit details returned by a completed eligibility inquiry - plan status, network status, copays, coinsurance, deductibles, and out-of-pocket maximums.

- **Human URL:** [https://docs.opkit.co](https://docs.opkit.co)
- **Base URL:** `https://api.opkit.co/v1`

#### Tags

- Benefits
- Coverage
- Insurance

#### Properties

- [Documentation](https://docs.opkit.co)
- [OpenAPI](openapi/opkit-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opkit.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opkit.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Opkit Payers API

List and retrieve the insurance carriers (payers) Opkit connects to across the United States, used to identify the correct payer when creating an eligibility inquiry.

- **Human URL:** [https://docs.opkit.co](https://docs.opkit.co)
- **Base URL:** `https://api.opkit.co/v1`

#### Tags

- Payers
- Insurance
- Directory

#### Properties

- [Documentation](https://docs.opkit.co)
- [OpenAPI](openapi/opkit-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opkit.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opkit.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Opkit Patients API

Create, retrieve, update, and list patient records used as the subject of eligibility inquiries, including demographics and member identifiers needed for verification.

- **Human URL:** [https://docs.opkit.co](https://docs.opkit.co)
- **Base URL:** `https://api.opkit.co/v1`

#### Tags

- Patients
- Records
- Healthcare

#### Properties

- [Documentation](https://docs.opkit.co)
- [OpenAPI](openapi/opkit-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opkit.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opkit.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Opkit Webhooks API

Register and manage webhook endpoints to receive event notifications - such as an eligibility inquiry completing - so applications can react to asynchronous results without polling.

- **Human URL:** [https://docs.opkit.co](https://docs.opkit.co)
- **Base URL:** `https://api.opkit.co/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.opkit.co)
- [OpenAPI](openapi/opkit-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opkit.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opkit.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/opkit)
- [Website](https://www.opkit.co)
- [Documentation](https://docs.opkit.co)
- [Plans](plans/opkit-plans-pricing.yml)
- [Rate Limits](rate-limits/opkit-rate-limits.yml)
- [Fin Ops](finops/opkit-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
