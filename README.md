# id-schemas

A collection of open, lightweight JSON Schemas
for representing common entities in Indonesia.

This repository focuses on real-world Indonesian contexts,
where informal operations, partial data, and WhatsApp-based
communication are common.

---

## Scope

This repository provides schemas for:

- Local business profiles
- Indonesian address structures (RT/RW, kelurahan, kecamatan)
- Geographic coordinates
- Business contact channels
- Opening hours and operational status

The schemas are designed to be:

- composable
- implementation-agnostic
- friendly to partial and evolving data

This is **not** an API, SDK, or application.
It defines **data contracts only**.

---

## Why id-schemas?

Global data schemas often assume:

- fully registered businesses
- complete addresses
- email-first communication
- rigid operating hours

In many Indonesian contexts, these assumptions do not hold.

`id-schemas` aims to provide a practical alternative
by reflecting how local businesses actually operate.

---

## Structure

```text
schemas/
├── business/
│ ├── profile.schema.json
│ ├── hours.schema.json
│ └── status.schema.json
├── address/
│ ├── address.schema.json
│ └── geo.schema.json
└── contact/
└── contact.schema.json

examples/
└── warung-lengkap.json
```

Each domain is documented in `schemas/README.md`.

---

## Usage

Schemas in this repository are intended to be combined
at the application or platform layer.

Example use cases:

- local business listings
- community directories
- chat-based commerce
- lightweight marketplaces
- data normalization pipelines

See the `examples/` directory for a complete business example.

---

## Design Principles

- **Context-aware**  
  Designed with Indonesian usage patterns in mind.

- **Flexible by default**  
  Partial data should still be valid data.

- **Separation of concerns**  
  Identity, address, location, hours, and status are independent.

- **No business logic**  
  Validation rules are intentionally minimal.

---

## Versioning

This repository follows Semantic Versioning (SemVer):

- MAJOR: breaking schema changes
- MINOR: backward-compatible additions
- PATCH: documentation or example updates

Schemas are versioned at the repository level.

---

## License

MIT License.
