# RRGI lexicons

This repository holds draft AT Protocol lexicons for the Resilient Research Graph Infrastructure (RRGI). We are still changing them, so a change may break records written against an earlier version.

Lexicon resolution does not work for these names yet. The domain `rrgi.scios.tech` has no `_lexicon` DNS record, which is how a resolver would find `com.atproto.lexicon.schema` records.

## Contents

`lexicons/` holds 31 schemas in the `tech.scios.rrgi.*` namespace:

- **Nodes:** claim, evidence, question, source, study, protocol, tradition, issue, and entity.
- **Relations:** supports, opposes, derivedFrom, contradicts, addresses, describes, grounds, follows, stemsFrom, equivalentTo, versionOf, observationStatement, observationOriginActivity, observationBase, and sourceDocument.
- **Stances and intent:** endorsement, attribution, and issueClaim.
- **Sets:** bundle and narrative.
- **Identity:** orcidLink.
- **Shared definitions:** defs.

Each file's `description` says what the type means and how it relates to MIRA.

This repository is a copy of those files from RRGI's private source repository, taken on 6 November 2026. Some descriptions mention RRGI documents, such as `LEXICONS.md`, that this repository leaves out. Others mention workshop record types, such as `group` and `accountList`, that are also missing.

## Where the schema comes from

These schemas implement the [MIRA community schema](https://github.com/MIRA-science/schema) (Apache-2.0) plus extensions that RRGI intends to propose upstream to MIRA.

The field shapes were first ported in May 2026 from [DiscourseGraphs/schemas](https://github.com/DiscourseGraphs/schemas) (CC0-1.0), which the files credit as their lineage.

MIRA's own draft lexicons, `science.mira.*`, are on the [`atproto-lexicon-draft` branch](https://github.com/MIRA-science/schema/tree/atproto-lexicon-draft/atproto/lexicons) of its repository.

## License

These files are available under the [Apache License 2.0](LICENSE), the same license as the MIRA schema.
