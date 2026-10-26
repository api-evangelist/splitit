# Splitit

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Splitit is a credit card installment platform that enables merchants to offer shoppers the ability to split existing credit card purchases into monthly installments without requiring new credit applications, additional interest charges, or third-party redirects. The platform operates directly on shoppers' existing credit cards, leveraging available credit to create installment plans while merchants receive full payment upfront.

**Developer Portal:** https://developers.splitit.com/

## APIs

| API | Description |
|-----|-------------|
| Installments API v3 | Create and manage credit card installment plans |
| Installments API v4 | Updated installment plan management |
| Account Management System API | Onboard and manage sub-merchants |
| Merchant Reports API | Retrieve transaction and funding reports |
| Key Exchange Server API | Manage encryption keys for secure integrations |
| Chargebacks API | Handle and respond to chargeback disputes |
| Text-to-Pay API | Initiate installment plans via SMS, email, and QR codes |

## Authentication

All API requests require Bearer token authentication. Obtain tokens via the identity server:

- **Sandbox:** `https://id.sandbox.splitit.com/connect/token`
- **Production:** `https://id.production.splitit.com/connect/token`

Token request uses OAuth 2.0 `client_credentials` grant with `client_id` and `client_secret` from your Merchant Hub.

## Base URLs

- **Sandbox:** `https://web-api-v3.sandbox.splitit.com`
- **Production:** `https://webapi.production.splitit.com`

## SDKs

Official SDKs available at https://github.com/splitit:

- Python: https://github.com/Splitit/Python-SDK
- TypeScript: https://github.com/Splitit/TypeScript-SDK
- Go: https://github.com/Splitit/Go-SDK
- Java: https://github.com/Splitit/Java-SDK
- .NET/C#: https://github.com/Splitit/.NET-C-SDK
- PHP: https://github.com/Splitit/PHP-SDK

## Merchant Plans

Splitit offers four merchant pricing tiers. See [plans/plans.yml](plans/plans.yml) for details.

| Plan | Consumer APR | Upfront Funding |
|------|-------------|-----------------|
| Essential | 0%–35.99% | Full |
| Flex | 0%–35.99% (variable) | Full |
| Premium | 0% | Full |
| Premium Lite | 0% | Partial |

All plans support up to $10,000 per order and up to 12 installments. Contact Splitit sales for merchant fee rates.

## Resources

- [APIs Overview](https://developers.splitit.com/apis/)
- [Quickstart Guide](https://developers.splitit.com/direct-api/quickstart/)
- [Sandbox Registration](https://register-developer.sandbox.splitit.com/)
- [Pricing Plans](https://www.splitit.com/business/pricing-plans/)
- [Trust Center](https://trust.splitit.com)
- [Merchant Portal](https://merchant.splitit.com)
- [Contact Sales](https://www.splitit.com/contact-sales/)

## Profile

This repository contains an [APIs.json 0.19](apis.yml) profile for Splitit maintained by [API Evangelist](https://apievangelist.com).
