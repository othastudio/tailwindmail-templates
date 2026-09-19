<p align="center">
  <img src=".github/ressources/logo-d.svg" alt="TailwindMail" width="320">
</p>

<p align="center">
  <strong>Build faster HTML emails with Tailwind CSS</strong>
</p>

<p align="center">
  Write clean Tailwind markup, compile it into responsive email-safe HTML,<br>
  and ship campaigns that work in Outlook, Gmail, and Apple Mail.
</p>

<p align="center">
  <a href="https://tailwindmail.dev">Website</a> ·
</p>

---

## What is this repository?

This is the **open-source template gallery** for [TailwindMail](https://tailwindmail.dev) a Tailwind-safe email writer and visual editor. Write emails in Tailwind, or build them with drag and drop, then compile to HTML that inboxes understand.

We publish official designs here, and anyone can share their own. Browse the live gallery at [tailwindmail.dev/templates](https://tailwindmail.dev/templates), fork a layout into the [editor](https://tailwindmail.dev/editor), or clone this repo and drop a template into your next campaign.

Use these templates for transactional mail, product updates, invoices, launches, and marketing emails. Every design is meant to compile with TailwindMail into HTML that works in Gmail, Outlook, and Apple Mail.

---

## Using a template

1. Open the [template gallery](https://tailwindmail.dev/templates) and pick a design.
2. Preview it, download the HTML, or **Fork to editor** on [TailwindMail](https://tailwindmail.dev).
3. Open it in the [editor](https://tailwindmail.dev/editor): edit the Tailwind source, or rearrange blocks with drag and drop. Then compile and send.

From this repo:

```bash
git clone https://github.com/othastudio/tailwindmail-templates.git
cd tailwindmail-templates
```

Each template is a folder at the repo root (`starter-template/`, then your own slug). Import `source.html` into [TailwindMail](https://tailwindmail.dev), or send `compiled.html` through Laravel, Node.js, Resend, Brevo, SendGrid, and similar providers.

New to the product? Start with the [TailwindMail docs](https://tailwindmail.dev/docs).

---

## Repository layout

```
README.md
starter-template/           Copy this folder as a reference
  meta.json                 Name, author, category, description
  source.html               Inner Tailwind markup (no html/body)
  compiled.html             Email-safe HTML (what you send)
  preview.png               Screenshot for the gallery
  README.md                 Optional notes
welcome-email/              Official welcome template
email-verification/         Official verify-email template
otp-code/                   Official OTP code template
magic-link/                 Official magic-link login template
password-reset/             Official password reset template
your-template-slug/         Your submission, same files as above
```

One folder per template, at the root. Credit yourself in `meta.json` that handle is what shows on [the gallery](https://tailwindmail.dev/templates).

---

## Share your template

We want this gallery to grow with real work from the community welcome emails, receipts, launch notes, newsletters, and anything else you have shipped with [TailwindMail](https://tailwindmail.dev).

### 1. Design it

Build it in [TailwindMail](https://tailwindmail.dev/editor) write Tailwind classes in the code editor, or drag and drop blocks. Compile, preview on desktop and mobile, then send a test before you submit.

### 2. Add it to the repo

Fork [othastudio/tailwindmail-templates](https://github.com/othastudio/tailwindmail-templates), create a branch, and add a folder at the **repo root**:

```
<your-template-slug>/
```

Copy [`starter-template/`](starter-template) as the reference it has every required file. Use a short kebab-case slug (`welcome`, `password-reset`, `weekly-digest`). Include:

| File | Required | Purpose |
| --- | --- | --- |
| `meta.json` | Yes | Gallery metadata |
| `source.html` | Yes | Inner Tailwind markup only (no `html` / `head` / `body`) |
| `compiled.html` | Yes | Compiled, inlined HTML |
| `preview.png` | Yes | 1200×900 (or similar) screenshot |
| `README.md` | Optional | Extra notes, credits, variants |

`meta.json` example:

```json
{
  "name": "Welcome aboard",
  "slug": "welcome-aboard",
  "author": "your-github-handle",
  "category": "transactional",
  "description": "A calm onboarding email with a single primary CTA."
}
```

Suggested categories: `transactional`, `onboarding`, `marketing`, `newsletter`, `receipt`, `alert`.

### 3. Open a pull request

Describe the use case, the clients you checked, and a screenshot. Once the PR is reviewed and merged, the template can appear in [Community templates](https://tailwindmail.dev/templates).

You can also start from the **Submit template** flow on [tailwindmail.dev/templates](https://tailwindmail.dev/templates).

### Guidelines

- Submit original work, or work you have the right to share under the repository license.
- Keep the layout email-safe: table-friendly structure, inline-friendly styles, a clear CTA.
- Avoid tracking scripts, remote fonts that break in Outlook, and huge images.
- Do not include private brand assets, customer data, or secrets.
- Credit yourself in `meta.json` community templates show your GitHub handle on the site.

---

## How to use TailwindMail

[TailwindMail](https://tailwindmail.dev) is a Tailwind-safe email writer and a visual editor. Write Tailwind markup, or drag and drop sections, buttons, and cards both compile to inlined HTML you can preview and export.

| Start here | Link |
| --- | --- |
| Product | [tailwindmail.dev](https://tailwindmail.dev) |
| Docs | [Installation, writing emails, compiling](https://tailwindmail.dev/docs) |
| Editor | [Write Tailwind or drag and drop](https://tailwindmail.dev/editor) |
| Template library | [Official and community designs](https://tailwindmail.dev/templates) |
| Changelog | [What shipped recently](https://tailwindmail.dev/changelog) |
| Source | [github.com/othastudio/tailwindmail](https://github.com/othastudio/tailwindmail) |

Typical flow: write Tailwind **or** drag and drop → compile → preview in Gmail / Outlook / Apple Mail → send. Details live in the [docs](https://tailwindmail.dev/docs) (`Write emails`, `Compile to HTML`, `Email clients`).

---

## Resources

Guides from the [TailwindMail blog](https://tailwindmail.dev/resources) on building, compiling, and testing HTML emails with Tailwind CSS.

### Get started

- [How to Build HTML Emails with Tailwind CSS](https://tailwindmail.dev/resources/how-to-build-html-emails-with-tailwind-css)
- [Can You Use Tailwind CSS in HTML Emails?](https://tailwindmail.dev/resources/can-you-use-tailwind-css-in-html-emails)
- [Tailwind CSS Email Templates: Examples, Components & How They Work](https://tailwindmail.dev/resources/tailwind-css-email-templates)
- [How to Convert Tailwind CSS to Email-Safe HTML](https://tailwindmail.dev/resources/how-to-convert-tailwind-css-to-email-safe-html)
- [Tailwind CSS Email Development Workflow](https://tailwindmail.dev/resources/tailwind-css-email-development-workflow)

### Editor and compile

- [How to Build HTML Emails with a Drag-and-Drop Editor](https://tailwindmail.dev/resources/how-to-build-html-emails-with-a-drag-and-drop-editor)
- [How to Inline Tailwind CSS for HTML Emails](https://tailwindmail.dev/resources/how-to-inline-tailwind-css-for-html-emails)
- [CSS Inlining in HTML Email](https://tailwindmail.dev/resources/css-inlining-in-html-email)
- [Responsive Tailwind CSS Emails](https://tailwindmail.dev/resources/responsive-tailwind-css-emails)

### Clients and testing

- [Tailwind CSS Email Compatibility: Gmail, Outlook & Apple Mail](https://tailwindmail.dev/resources/tailwind-css-email-compatibility)
- [How to Make Tailwind CSS Emails Work in Outlook](https://tailwindmail.dev/resources/how-to-make-tailwind-css-emails-work-in-outlook)
- [HTML Email Testing: Gmail, Outlook, Apple Mail & Mobile](https://tailwindmail.dev/resources/html-email-testing)
- [Why Tailwind CSS Doesn't Work Directly in Every Email Client](https://tailwindmail.dev/resources/why-tailwind-css-doesnt-work-directly-in-every-email-client)

### Components and comparisons

- [Tailwind CSS Email Buttons](https://tailwindmail.dev/resources/tailwind-css-email-buttons)
- [Tailwind CSS Email Dark Mode](https://tailwindmail.dev/resources/tailwind-css-email-dark-mode)
- [React Email vs MJML vs TailwindMail](https://tailwindmail.dev/resources/react-email-vs-mjml-vs-tailwindmail)
- [Best HTML Email Builders for Developers in 2026](https://tailwindmail.dev/resources/best-html-email-builders-for-developers-2026)

More articles, tagged by topic: [tailwindmail.dev/resources](https://tailwindmail.dev/resources).

---

## License

Templates in this repository are shared so the community can learn from them, fork them, and ship faster. By opening a pull request you confirm that you can license your submission the same way, and that [TailwindMail](https://tailwindmail.dev) may feature it in the public gallery.

Questions or ideas? Open an issue on this repo, or visit [tailwindmail.dev](https://tailwindmail.dev).
