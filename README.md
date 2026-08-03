# ProvKOS — Publication Repository

This repository serves the **published version** of the ProvKOS ontology and its human-readable documentation at the persistent namespace URI:

**https://w3id.org/def/ProvKOS**

ProvKOS is an Application Profile extending W3C [SKOS](https://www.w3.org/TR/skos-reference/) and [PROV-O](https://www.w3.org/TR/prov-o/) to document the provenance of editorial activities in Knowledge Organization Systems (KOS): typed change activities, warrant structures, and the relationships among entities, activities, agents, and warrants.

## Contents

| Path | Description |
|---|---|
| `ProvKOS.owl` | Published ontology (RDF/XML serialization of the current release). |
| `OnToology/ProvKOS.owl/documentation/` | Human-readable documentation (WIDOCO), served via GitHub Pages. |

Development — ontology sources in Turtle, case-study datasets, SHACL shapes, and validation scripts — happens in **[cik860/ProvKOS](https://github.com/cik860/ProvKOS)**. Please open issues and pull requests there.

## Current release

**v1.1** (2026). Changes from v1.0, made during peer-review revision:

- Class renamed `ProvKOS:ClassNumber` (formerly `Class_number`)
- Domain of `ProvKOS:hasLabel` broadened to `prov:Entity`, so labels attach to non-notation KOS entities such as authority records
- Explicit PROV-O sub-property alignments: `wasDeprecatedBy` ⊑ `prov:wasInvalidatedBy`, `wasAuthorizedBy` ⊑ `prov:wasGeneratedBy`, `wasWarrantedBy` ⊑ `prov:wasInfluencedBy`
- `skos:Concept` and `skos:ConceptScheme` declared as subclasses of `ProvKOS:Warrant`, with scope notes
- Added `ProvKOS:documentDate` and `ProvKOS:documentURI` for Document warrants
- Example individuals moved to the development repository's `data/` directory

## Citation

> Choi, I., & Cheng, Y.-Y. ProvKOS: An Application Profile for Documenting Provenance in Knowledge Organization Systems. *(under review)*

## Authors

- Inkyung Choi — Sungkyunkwan University ([ORCID 0000-0001-5048-8516](https://orcid.org/0000-0001-5048-8516))
- Yi-Yun Cheng — Rutgers University ([ORCID 0000-0001-6123-7595](https://orcid.org/0000-0001-6123-7595))
