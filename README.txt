TENIR Schemas v1.0 (Publishable Bundle)

Structure:
  schemas/v1/*.schema.json
  openapi/tenir-engine.openapi.yaml

Notes:
- This bundle is designed for public publishing under a stable URL root:
    https://schemas.tenir.example.com/v1/
- References are relative file references (e.g. system-entity.schema.json).
- Some schemas are "stubs" (Scenario, Recommendation, etc.) intended to be expanded as the engine matures.
  They are valid Draft 2020-12 JSON Schemas and keep the bundle consistent.

Recommended hosting:
- Static hosting (S3/GCS + CDN) with immutable versioned path.
- Add Content-Type: application/schema+json for *.schema.json files.
