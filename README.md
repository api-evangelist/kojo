# Kojo

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
