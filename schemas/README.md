# Schemas Overview

This directory contains a collection of open JSON Schemas
for representing common entities in Indonesia.

Each schema is designed to be:

- lightweight
- composable
- context-aware for Indonesian use cases

Schemas are grouped by domain and intended to be combined
at the application layer.

---

## Business Domain (`business/`)

Schemas related to business identity and operations.

### `profile.schema.json`

Core business identity.

Common fields:

- `business_name`
- `legal_name`
- `category`
- `tags`

This schema represents **what the business is**.

---

### `hours.schema.json`

Planned business opening hours.

- Supports different hours per day
- Allows multiple time ranges per day
- Includes optional human-readable notes

This schema represents **when the business is expected to operate**.

---

### `status.schema.json`

Current operational status.

- `state`: open / closed / unknown
- `last_updated`: ISO timestamp
- `source`: manual / system / bot

This schema represents **the current real-world condition**.

---

## Address Domain (`address/`)

Schemas for representing Indonesian addresses and locations.

### `address.schema.json`

Text-based address structure.

- RT / RW supported
- Kelurahan and kecamatan included
- No required fields (partial addresses allowed)

This schema represents **where the business is described to be**.

---

### `geo.schema.json`

Geographic coordinates.

- Latitude and longitude only
- Strict numeric bounds
- Optional and independent from address

This schema represents **where the business is physically located**.

---

## Contact Domain (`contact/`)

Schemas for business communication channels.

### `contact.schema.json`

Primary contact information.

- WhatsApp-first
- Email and website optional
- No format enforcement beyond basic validation

This schema repres
