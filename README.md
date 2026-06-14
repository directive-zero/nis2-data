# Open NIS2 Dataset

Machine-readable NIS2 reference data for Germany / BSIG, extracted from the Directive Zero v1 browser tools.

The canonical data lives in `data/*.json`:

- `data/scope.json` covers affectedness logic, special cases, sectors, size thresholds, and result rows.
- `data/obligations.json` covers the §30 / §38 / §32 obligations matrix and assessment items.
- `data/deadlines.json` covers statutory clocks for incident reporting, registration, and change notifications.

Generated Markdown tables in `dist/` are citation-oriented renderings of the JSON. They are built from the JSON and should not be edited by hand.

## Use

```sh
npm install @directive-zero/nis2-data
```

```js
import scope from "@directive-zero/nis2-data/scope";
import obligations from "@directive-zero/nis2-data/obligations";
import deadlines from "@directive-zero/nis2-data/deadlines";
```

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
