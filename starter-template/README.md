# Starter template

Reference layout for templates in this repository. Duplicate this folder when you add a new design.

| File | Required | What it is |
| --- | --- | --- |
| `meta.json` | Yes | Gallery name, slug, author, category, description |
| `source.html` | Yes | Inner Tailwind markup only (no `html` / `head` / `body`) |
| `compiled.html` | Yes | Inlined, table-based HTML you send |
| `preview.png` | Yes | Screenshot of the compiled email (~1200×900) |
| `README.md` | Optional | Notes for this template |

## Use it

1. Copy `source.html` into the [TailwindMail editor](https://tailwindmail.dev/editor).
2. Change copy, colors, and the CTA.
3. Compile, then replace `compiled.html` and `preview.png`.
4. Update `meta.json` (`name`, `slug`, `author`, `category`, `description`).

Add your own template as a new folder next to this one at the repo root (`welcome/`, `password-reset/`, …). See the [repo README](../README.md) for the full checklist.
