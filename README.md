# Splitit

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
