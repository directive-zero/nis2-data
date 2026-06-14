# Open NIS2 Dataset

**Short answer:** Machine-readable NIS2 reference data for Germany / BSIG — scope logic, §30 obligations, and statutory deadlines — published as versioned JSON under EUPL-1.2 and consumed by [directive0.eu](https://directive0.eu).

The live site renders from this data. The tables and tools on directive0.eu and the JSON files here are the same source.

## Canonical pages

| Data file | What it covers | Live page |
|-----------|----------------|-----------|
| [`data/scope.json`](data/scope.json) | Affectedness logic, sectors, thresholds, special cases | [NIS2-Betroffenheits-Check](https://directive0.eu/nis2/betroffenheit/) |
| [`data/obligations.json`](data/obligations.json) | §30 / §38 / §32 obligations matrix | [§30 Pflichten-Matrix](https://directive0.eu/nis2/pflichten/) |
| [`data/deadlines.json`](data/deadlines.json) | Incident reporting, registration, change clocks | [DACH deadlines](https://directive0.eu/nis2/fristen/) |
| Glossary (site inline for now) | Defined terms with legal references | [NIS2 glossary](https://directive0.eu/glossar/nis2/) |

## Use

```sh
npm install @directive-zero/nis2-data
```

```js
import scope from "@directive-zero/nis2-data/scope";
import obligations from "@directive-zero/nis2-data/obligations";
import deadlines from "@directive-zero/nis2-data/deadlines";
```

Generated Markdown tables in `dist/` are citation-oriented renderings of the JSON. They are built from the JSON and should not be edited by hand.

## Build

```sh
npm run build
npm run validate
```

## Legal Note

This dataset structures public statutory facts and Directive Zero's operationalized assessment wording. It is not legal advice, a certificate, or a conformity assessment. The law and official guidance remain authoritative.

Potentially near-verbatim legal or BSI-adjacent wording is tracked in `LEGAL_REVIEW.md` for review before broader promotion.

## License

EUPL-1.2. See `LICENSE`.

## Cite

See `CITATION.cff` — GitHub renders a "Cite this repository" button from this file.
