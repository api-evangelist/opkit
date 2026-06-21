# Opkit (opkit)

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
