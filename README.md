# Kojo

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

Kojo (formerly Agora) is a construction materials management and procurement platform for specialty trade contractors — electrical, mechanical, concrete, drywall, flooring, and roofing. It connects the field, purchasing, the warehouse, the prefab shop, and accounting into one materials workflow: requesting, sourcing, purchasing, receiving, tool tracking, invoice matching, and payment.

- Website: https://www.usekojo.com
- Application: https://kojo.app/login
- Help Center: https://support.usekojo.com/hc/en-us
- Backed by: 8vc

## API posture

**Kojo publishes no public, self-service developer API.** There is no OpenAPI, no API reference, and no developer portal; `developer.usekojo.com`, `docs.usekojo.com`, and `api.usekojo.com` do not resolve, and no `/.well-known/` discovery documents are served on any Kojo host.

What Kojo does have is a real, documented, partner-gated integration surface — the **Kojo Vendor Integration Portal**:

- **ANSI ASC X12 EDI** with supplier ERPs: 810 (Invoice), 840 (RFQ), 843 (Quote), 850 (Purchase Order), 855 (PO Acknowledgement), with a filterable EDI transaction log and raw file download.
- **Scheduled email file feeds** for catalog, price lists, and branch-level inventory availability (single `.csv`/`.txt` attachment, vendor-configured header rows).
- **API integration** — referenced in vendor documentation as an alternative to EDI, but with no published endpoints, hosts, auth scheme, or schemas. Arranged directly with Kojo via `vendor-integrations@usekojo.com`.
- **26 published integrations** across ERP/project-management systems and material distributors.

## Artifacts

| Artifact | File |
|---|---|
| Integration conventions | `conventions/kojo-conventions.yml` |
| Conformance (X12, SOC 2) | `conformance/kojo-conformance.yml` |
| Integrations catalog | `integrations/kojo-integrations.yml` |
| Trust center | `security/kojo-trust-center.yml` |
| Domain security | `security/kojo-domain-security.yml` |
| Well-known probe | `well-known/kojo-well-known.yml` |
| llms.txt | `llms/kojo-llms.txt` |
