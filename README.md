# Food and Drug Administration (food-and-drug-administration)

openFDA is an Elasticsearch-based public API that serves FDA data on drugs,
devices, foods, animal/veterinary products, and tobacco. Each noun exposes
one or more datasets including adverse events, recall enforcement reports,
product labeling, classifications, registrations, and approvals. Every query
goes through one endpoint for one kind of data.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Drugs, Devices, Federal Government, Food Safety, Public Data, Recalls, Adverse Events

## APIs

### openFDA

- **Human URL:** https://open.fda.gov/apis
- **Base URL:** https://api.fda.gov
- **Authentication:** Free API key via query parameter `api_key` (rate limits: 240 req/min, 120,000 req/day with key; 1,000 req/day per IP without key).

#### Endpoint families

- Drug: `/drug/event.json`, `/drug/label.json`, `/drug/enforcement.json`, `/drug/ndc.json`, `/drug/drugsfda.json`, `/drug/shortages.json`
- Device: `/device/event.json`, `/device/enforcement.json`, `/device/recall.json`, `/device/classification.json`, `/device/510k.json`, `/device/pma.json`, `/device/registrationlisting.json`, `/device/udi.json`, `/device/covid19serology.json`
- Food: `/food/enforcement.json`, `/food/event.json`
- Animal & Veterinary: `/animalandveterinary/event.json`
- Tobacco: `/tobacco/problem.json`
- Other: `/other/nsde.json`, `/other/substance.json`, `/other/historicaldocument.json`

## Machine-readable artifacts

- [OpenAPI 3.0](./openapi/openfda-openapi.yml)
- [Capabilities](./capabilities/openfda-capabilities.yml)
- [Rules](./rules/openfda-rules.yml)

## Common Properties

- [Website](https://www.fda.gov/)
- [Documentation](https://open.fda.gov/apis)
- [Authentication](https://open.fda.gov/apis/authentication/)
- [Terms of Service](https://open.fda.gov/terms/)
- [GitHub](https://github.com/FDA/openfda)

## Maintainers

- **FN:** Kin Lane
- **Email:** kin@apievangelist.com
