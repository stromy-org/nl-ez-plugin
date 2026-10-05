# EZK — Brand Guidelines

> **Derived view.** `charter.json` is the machine-readable source of truth; this file
> presents the same data for humans plus the usage context that does not fit in JSON.
> Regenerate whenever a charter promotion changes colours, fonts, logos or grammar.
>
> **Third-party brand.** The Rijkshuisstijl is the Dutch government's house style,
> not a Stromy-owned identity. This is *our working model*, recovered from public
> evidence (rijksoverheid.nl, 2026-10-03) and the charter's own provenance. The
> official guide at rijkshuisstijl.nl is **login-gated** and was not readable, so
> where EZK or the Rijkshuisstijl team supplies it, that supersedes this document.

Tier 2 (output) · Entity: Ministerie van Economische Zaken en Klimaat (EZK)

---

## 1. Foundation

| | |
|---|---|
| **Name** | Ministerie van Economische Zaken en Klimaat (EZK) |
| **Self-description** | "EZK werkt aan een productieve, weerbare en duurzame economie." (rijksoverheid.nl, 2026-10-03) |
| **Tagline** | De Rijksoverheid. Voor Nederland. |
| **Brand system** | Rijkshuisstijl (Dutch Government House Style) |
| **Domain** | rijksoverheid.nl — the ministry has no standalone domain |

**Both portfolios sit under one ministry.** *Minister van Economische Zaken en
Klimaat* and *Minister van Klimaat en Groene Groei* are portfolios of the same
ministry; no separate ministry exists (charter `meta.verification_notes`). Never
describe EZK and KGG as two ministries.

## 2. Colour

| Role | Name | Hex |
|---|---|---|
| Primary | Donkerblauw (Rijksblauw) | `#154273` |
| Secondary | Hemelblauw | `#01689b` |
| Accent | Geel | `#ffb612` |
| Text | — | `#1D1D1B` |
| Text, light | — | `#535353` |
| Surface | — | `#f3f3f3` |
| Border | — | `#e6e6e6` |
| Success / Warning / Error | — | `#39870c` / `#e17000` / `#c63c2c` |

Official Rijkshuisstijl palette (charter provenance, 2026-06-15). Brandfetch
returned `#154273` mislabelled as an accent for the umbrella record; do not take
colour roles from it. Links use Hemelblauw on white.

## 3. Typography

| Role | Official | Embedded substitute |
|---|---|---|
| Heading, body | RO Sans | Fira Sans (OFL) |
| Serif, long-form | RO Serif | Source Serif 4 (OFL) |

RO Sans and RO Serif are Rijksoverheid-licensed and ship **web-only** (woff2), so
they cannot be embedded in OOXML or PDF. Server-side renders embed the OFL
substitute, so a deliverable is self-contained; a machine with the RO fonts
installed still shows the named family. Fallback order: Segoe UI, Verdana, Arial,
sans-serif. Use the serif for formal reports and long-form body text.

## 4. Logo

The Dutch coat of arms (crowned lion) on a Rijksblauw `#154273` banner; the blue is
baked into the SVG. Use `logos/logo-wordmark.svg` for document headers and title
slides, `logos/logo.svg` where the vertical banner fits, at most 160 × 60 pt in a
header. The SVGs are byte-identical to the live Rijksoverheid sources
(verified 2026-05-19). Do not recolour, crop, stretch or rebuild the mark.

## 5. Imagery

`images/manifest.json` catalogues the cover and section photography. Photography is
documentary and institutional, not stock-lifestyle. Heroes for a specific
publication are **not** in the library yet: ask the colleague for approved
imagery rather than inventing a house look.

## 6. Voice and language

See `voice/voice-profile.md` and `voice/voice-anchors.md`. In short: Dutch by
default for Dutch-administration audiences, short active sentences, every claim tied
to its record, and no finding presented as an EZK position.

## 7. Open items

- **Templates.** Only docx (letterhead, styles), pdf and pptx fragments exist. There
  is no EZK-supplied deck master; request one from the colleague.
- **Rijkshuisstijl detail.** Spacing, grid and lint rules sit behind the login at
  rijkshuisstijl.nl; none are modelled here.
- **People.** There is no `people.json`; no contact is recorded.
