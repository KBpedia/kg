# KBpedia Knowledge Graph — kg Repository

**Note:** This repository is under active development for v3.00 (planned Fall 2026). The current public release is v2.50. Download the v2.50 OWL files from kbpedia.org/resources/downloads/.

## Overview

This repository contains the **source files and build artifacts** for the
KBpedia knowledge graph: CSV build inputs, typology files, external source
mappings, properties, and versioned archives of prior releases.

It is intended for developers and researchers who want to understand, build
upon, or contribute to the KBpedia knowledge graph construction process.

---

## Downloading KBpedia OWL Files

**If you want to use KBpedia** rather than build it, download the compiled
OWL files directly from the KBpedia website:

- KBpedia Reference Concepts: `kbpedia_reference_concepts.owl`
- KBpedia Knowledge Ontology: `kko.owl`

**Download page:** https://kbpedia.org/resources/downloads/

The OWL files are not stored in this repository due to their size (~150 MB).
They are built from the source files here using the
[cowpoke](https://github.com/KBpedia/cowpoke) roundtripping package.

---

## Repository Structure

```
kg/
├── v250/           # KBpedia v2.50 archive (public release, 2020)
├── v300/           # KBpedia v3.00 archive (added on release)
└── working/        # Active development version
    ├── build/      # CSV inputs to the build process
    ├── extract/    # Outputs extracted from the built ontology
    └── fixes/      # Changelog and supporting reference files
```

The `working/` directory always contains the version currently in
development. On public release it is renamed to the version number
(e.g., `v300/`) and a fresh `working/` stub is created for the next cycle.

---

## Versioning

| Version | Status | Release |
|---------|--------|---------|
| v2.50 | Public | June 2020 |
| v3.00 | In development | Planned Fall 2026 |

---

## Related Repositories

| Repo | Purpose |
|------|---------|
| [KBpedia/cowpoke](https://github.com/KBpedia/cowpoke) | Build/extract Python package |
| [KBpedia/wikidata](https://github.com/KBpedia/wikidata) | Wikidata harvest and upload tools |
| [KBpedia/kbpedia-site](https://github.com/KBpedia/kbpedia-site) | kbpedia.org website and API |

---

## License

KBpedia is open source. See individual version directories for license
details. The v3.00 license will be posted on release.

---

## About

KBpedia is a comprehensive knowledge graph and ontology framework integrating
Wikidata, Wikipedia, and other major knowledge sources into a coherent
structure grounded in Charles Sanders Peirce's universal categories.

**Author:** Michael K. Bergman
**Publisher:** Semantics Press LLC
**Website:** https://kbpedia.org
**Blog:** https://www.mkbergman.com
