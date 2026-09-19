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
  <a href="https://github.com/othastudio/tailwindmail">GitHub</a>
</p>

---

## What is this repository?

This is the **open-source template gallery** for [TailwindMail](https://tailwindmail.dev) — a visual email builder and compiler for people who already think in Tailwind.

We publish official designs here, and anyone can share their own. Browse the live gallery at [tailwindmail.dev/templates](https://tailwindmail.dev/templates), fork a layout into the [editor](https://tailwindmail.dev/editor), or clone this repo and drop a template into your next campaign.

Use these templates for transactional mail, product updates, invoices, launches, and marketing emails. Every design is meant to compile with TailwindMail into HTML that works in Gmail, Outlook, and Apple Mail.

---

## Using a template

1. Open the [template gallery](https://tailwindmail.dev/templates) and pick a design.
2. Preview it, download the HTML, or **Fork to editor** on [TailwindMail](https://tailwindmail.dev).
3. Customize copy, colors, and blocks in the [visual editor](https://tailwindmail.dev/editor), then compile and send.

From this repo:

```bash
git clone https://github.com/othastudio/tailwindmail-templates.git
cd tailwindmail-templates
```

Each template lives in `templates/` with Tailwind source, compiled HTML, and a preview. Import the source into [TailwindMail](https://tailwindmail.dev), or send the compiled HTML through Laravel, Node.js, Resend, Brevo, SendGrid, and similar providers.

New to the product? Start with the [TailwindMail docs](https://tailwindmail.dev/docs).

---

## Repository layout

```
templates/
  official/                 Official TailwindMail templates
    barebone/
      meta.json             Name, author, category, description
      source.html           Tailwind markup (what you edit)
      compiled.html         Email-safe HTML (what you send)
      preview.png           Screenshot for the gallery
  community/                Community submissions
    your-github-handle/
      invoice-notice/
        ...
```

Official templates are maintained by the TailwindMail team. Community templates are grouped by GitHub username so authors stay credited on [the gallery](https://tailwindmail.dev/templates).

---

## Share your template

We want this gallery to grow with real work from the community — welcome emails, receipts, launch notes, newsletters, and anything else you have shipped with [TailwindMail](https://tailwindmail.dev).

### 1. Design it

Build the email in the [TailwindMail editor](https://tailwindmail.dev/editor), or write Tailwind markup by hand and compile it. Preview on desktop and mobile, then send a test before you submit.

### 2. Add it to the repo

Fork [othastudio/tailwindmail-templates](https://github.com/othastudio/tailwindmail-templates), create a branch, and add a folder:

```
templates/community/<your-github-handle>/<template-slug>/
```

Use a short kebab-case slug (`welcome`, `password-reset`, `weekly-digest`). Include:

| File | Required | Purpose |
| --- | --- | --- |
| `meta.json` | Yes | Gallery metadata |
| `source.html` | Yes | Tailwind source |
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
  "description": "A calm onboarding email with a single primary CTA.",
  "tags": ["welcome", "onboarding"],
  "clients": ["gmail", "outlook", "apple-mail"]
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
- Credit yourself in `meta.json` — community templates show your GitHub handle on the site.

---

## How to use TailwindMail

[TailwindMail](https://tailwindmail.dev) compiles Tailwind utility classes into inlined, email-safe HTML. You can drag blocks in the editor, paste Tailwind source, preview live, and export HTML for your stack.

| Start here | Link |
| --- | --- |
| Product | [tailwindmail.dev](https://tailwindmail.dev) |
| Docs | [Installation, writing emails, compiling](https://tailwindmail.dev/docs) |
| Editor | [Build and preview in the browser](https://tailwindmail.dev/editor) |
| Template library | [Official and community designs](https://tailwindmail.dev/templates) |
| Changelog | [What shipped recently](https://tailwindmail.dev/changelog) |
| Source | [github.com/othastudio/tailwindmail](https://github.com/othastudio/tailwindmail) |

Typical flow: write Tailwind markup → compile → preview in Gmail / Outlook / Apple Mail → send. Details live in the [docs](https://tailwindmail.dev/docs) (`Write emails`, `Compile to HTML`, `Email clients`).

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
