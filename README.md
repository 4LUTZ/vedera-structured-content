# Vedera Structured Content – Sitemap

Dieses Repository enthält eine strukturierte Repräsentation der Sitemap von [vedera.de](https://vedera.de).

## Struktur

- `data/vedera-sitemap.json`  
  Enthält die vollständige Sitemap-Struktur (Seiten, Kategorien, Hersteller, News, Footer).

- `schema/vedera-sitemap.schema.json`  
  JSON Schema zur Validierung der Sitemap-Struktur.

## Validierung

Beispiel (Node.js mit `ajv`):

```bash
npm install ajv ajv-cli
npx ajv validate -s schema/vedera-sitemap.schema.json -d data/vedera-sitemap.json
