## Network of Trusted Networks - Event Schemas

This repository contains JSON Schemas for events used in the **Network of Trusted Networks**.

- **HTML catalog**: `index.html` – human-readable overview of available event schemas.
- **Schemas**: versioned under folders such as `v0.1/`.
- **Schema index**: `v0.1/index.json` – machine-readable registry of schemas for a given version.

### Repository layout

- `index.html` – landing page listing event codes, names, and links to their schema files.
- `header.css` – minimal styling for the landing page.
- `v0.1/` – JSON Schemas for version 0.1 of the event model.

### Usage

- Use the JSON Schema files under `v0.1/` (and future `vX.Y/` folders) to validate event payloads.
- Use `v0.1/index.json` as a registry to programmatically discover schemas and their canonical URLs.
- When adding new events:
  - Add or update the schema in the appropriate version folder.
  - Update the version-specific `index.json` registry.
  - Update `index.html` (or any future generated catalog) to reflect the new event.

### Contributing

Contributions are welcome:

- Discuss changes via issues or pull requests before large modifications.
- Keep schemas backward compatible when possible, or clearly document breaking changes.
- Ensure any new or changed schemas are valid JSON Schema and, ideally, include example payloads.

### License

The content of this repository is provided under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license (see `LICENSE` for details). This allows use, sharing, and modification for **any purpose, including commercial use**, provided attribution is given.

