# workspace-contracts

Alpha 0.1.0-alpha.8; Apache-2.0. Not for production use.

Provider-neutral JavaScript and Python contracts for workspace collaboration, qualified identities, projects, collections, immutable documents, retained evidence and releases. JSON schemas and fixed identity conformance fixtures are included.

JavaScript imports use `@categori/workspace-contracts` and its declared subpath exports. Python imports use `categori_workspace_contracts` after adding `python/` to the import path. The APIs and version are recorded in `package.json`.

A collection has its own identity and revision. Its descriptive owner can be a User, Team or Organization; agency/client contexts and audience intent are explicit. Collection metadata does not grant access to members. Applications independently enforce current identity, membership, provider access and resource policy.

Immutable document links use qualified immutable references, byte lengths and SHA-256 integrity manifests. Complete-byte verification does not fetch content or authorize publication. Conflicting integrity metadata for an existing version must be rejected.

The included demo/publication contracts constrain a curated MassGIS-only alpha scope. They are policy records and validators, not a hosted demo or a production authorization service. Fixtures contain synthetic identifiers and public source references; no datasets are redistributed. Application-specific adapters are outside this repository.

Registry packages are not published by this source release. Node manifests retain `private: true` to guard against accidental npm publication. See the repository CI for offline test commands.
