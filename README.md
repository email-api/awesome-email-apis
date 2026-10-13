# Awesome Email APIs

A curated list of **hosted email APIs and related developer tools** for sending email from applications.

This list is for builders adding password resets, receipts, magic links, and product notifications—not for newsletter design systems or drag-and-drop template galleries.

**Related (different jobs):**

- Fundamentals: [email-api/email-api-guide](https://github.com/email-api/email-api-guide)
- Recommendation guide: [transactional-email/best-transactional-email-apis](https://github.com/transactional-email/best-transactional-email-apis)
- HTML email design lists: [awesome-emails](https://github.com/eric-erki/awesome-emails) (frameworks/templates)
- Open-source servers: [awesome-opensource-email](https://github.com/Mindbaz/awesome-opensource-email)

## Contents

- [Transactional / developer email APIs](#transactional--developer-email-apis)
- [Broader email platforms](#broader-email-platforms)
- [Self-hosted send platforms](#self-hosted-send-platforms)
- [Testing and local catchers](#testing-and-local-catchers)
- [How to choose](#how-to-choose)
- [Inclusion criteria](#inclusion-criteria)
- [Contributing](#contributing)

Entries within each section are **alphabetical**. Hosted SaaS is not labelled as open source.

## Transactional / developer email APIs

Hosted HTTP APIs aimed at application email (send + typically webhooks/logs).

- [Amazon SES](https://aws.amazon.com/ses/) — AWS email sending service; low unit cost at scale; you assemble DX (logging, webhooks, domain UX) yourself. New accounts may face production access delays.
- [Mailgun](https://www.mailgun.com/) — Developer email API with sending, inbound routes, and validation products.
- [Notify](https://notify.cx) — Minimal transactional email API (send, domain auth, logs, webhooks). Clients: `fetch`, [`notifycx`](https://github.com/notifycx/notifycx) SDK, [`notifycx-mcp`](https://notify.cx/mcp). Source: [notifycx/notifycx](https://github.com/notifycx/notifycx).
- [Postmark](https://postmarkapp.com/) — Transactional-focused email API known for deliverability tooling and message streams.
- [Resend](https://resend.com/) — Modern developer email API; Node/React Email–oriented DX; broader product surface than send-only APIs.
- [SendGrid](https://sendgrid.com/) — Twilio email platform; transactional + marketing in one ESP-style product.
- [SparkPost](https://www.sparkpost.com/) — High-volume email delivery API (Bird/SparkPost).

## Broader email platforms

Products that include transactional sending plus marketing, automation, or CRM surfaces. Useful if you need those features; heavier if you only need app email.

- [Brevo](https://www.brevo.com/) (formerly Sendinblue) — Marketing + transactional email with CRM/automation options.
- [Mailchimp Transactional](https://mailchimp.com/developer/transactional/) (Mandrill) — Transactional add-on in the Mailchimp ecosystem.
- [Mailjet](https://www.mailjet.com/) — Email API and marketing tools under Sinch.

## Self-hosted send platforms

Open-source or self-hosted systems. You operate infrastructure, reputation, and compliance. Prefer [awesome-opensource-email](https://github.com/Mindbaz/awesome-opensource-email) for a deeper catalog.

- [Postal](https://github.com/postalserver/postal) — Self-hosted mail delivery platform for incoming and outgoing email.
- [Zone-MTA](https://github.com/zone-eu/zone-mta) — Modern outbound MTA (Node.js), extendable for custom sending pipelines.

## Testing and local catchers

- [MailHog](https://github.com/mailhog/MailHog) — Local SMTP catcher with web UI (legacy but widely referenced).
- [Mailpit](https://github.com/axllent/mailpit) — Modern local email testing tool (SMTP + UI + API).
- [Mailtrap](https://mailtrap.io/) — Hosted email testing / sandbox for safe previews without hitting real users.
- [caniemail](https://www.caniemail.com/) — HTML/CSS support tables for email clients (not a send API).

## How to choose

1. Read [email-api-guide](https://github.com/email-api/email-api-guide) for HTTP vs SMTP and evaluation dimensions.
2. Use [best-transactional-email-apis](https://github.com/transactional-email/best-transactional-email-apis) for use-case recommendations (Next.js, indie SaaS, coding agents, alternatives).
3. Prefer a **minimal transactional** API when you already render HTML and only need send + domain auth + logs/webhooks.
4. Prefer an **ESP** when you also need marketing campaigns, audiences, and visual builders in the same vendor.

## Inclusion criteria

See [CONTRIBUTING.md](./CONTRIBUTING.md). Short version: official link, factual description, correct hosted vs OSS labelling, relevant to app developers.

## Contributing

PRs welcome. Please read [CONTRIBUTING.md](./CONTRIBUTING.md).

## License

[MIT](./LICENSE)

## Transparency

This repository is maintained by the same owner as [Notify](https://notify.cx). The directory aims to be useful and accurate for the ecosystem; Notify is listed alphabetically among peers, not pinned above them in the catalogs above.
