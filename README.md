# Postman Collections

You can use the following Postman collections to interact with the **Ratepay APIs** in the **integration environment**.

The collections cover common payment flows and can be used as a reference or starting point for custom integrations.

## Covered APIs

- **Payment API 2.0 (JSON)**
  - Authorization
  - One Time Passcode (Validate & Regenerate)
  - Capture
  - Refund
  - Cancellation
  - Incremental Authorization
  - Shipping Information
- **Payment API 1.8 (XML)**
  - PROFILE_REQUEST (get configuration for specified credentials)
  - CONFIGURATION_REQUEST (get configuration for Pay in 3)
  - CALCULATION_REQUEST (for Pay in 3)
  - PAYMENT_INIT (Initialization)
  - PAYMENT_REQUEST (Authorization)
  - PAYMENT_CONFIRM (Handshake)
  - CONFIRMATION_DELIVER (Capture)
  - PAYMENT_CHANGE (change-order, credit, cancellation, return)
- **Hosted Payment Page (HPP)**
  - Create session
  - Receive session record(s)
- **Transaction Status API**
  - Get order status

---

## Getting Started

### 1. Import the Collections
Import the `Ratepay Payment API 2.0 (Integration).postman_collection.json` and/or `Ratepay Payment API 1.8 (Integration).postman_collection.json` into Postman.

### 2. Test Data & Credentials

The collections comes with generally available public credentials & is ready-to-use.

All other variables (tokens, IDs) are set automatically by test scripts.

Included personal data (names, addresses, IBANs, emails...) are fictional test data.

No production data is used.

---

## Authentication

Most APIs use **OAuth 2.0 Client Credentials**.

Run the following request first:
```text
0 - 🔑 Request OAuth Token
```

The access token is automatically stored and reused by subsequent requests.

---

## Notes
Base URLs point to the integration environment

This collections are intended for demonstration and testing purposes