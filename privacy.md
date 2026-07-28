---
version: "2026-07-28"
title: Mizu — Privacy Policy
last_updated: July 28, 2026
---

# Mizu — Privacy Policy

Last updated: July 28, 2026

## 1. Who We Are

Mizu is a personal spending tracker provided by DMC Labs, LLC
("DMC Labs," "we," "us," or "our"). This Privacy Policy explains what
information Mizu collects, how we use it, and the choices you have.

## 2. Information We Collect

### 2.1 Account information

When you sign in with Sign in with Apple, we receive your name and
email address; you may choose Apple's Hide My Email option, in which
case we receive only an Apple-provided relay email address. If you
sign in with an email address and password instead, we store your
email address and a securely hashed password. We never see your
Apple password.

### 2.2 Financial transaction data

We receive transaction data from your bank through Plaid, a regulated
bank-data aggregator acting on your behalf. We receive: account name,
account type, the last four digits of the account number, individual
transaction date, amount, merchant description, and posting metadata.
We do **not** receive your bank login credentials at any time. We do
**not** have the ability to move money — the connection is read-only.

Transaction descriptions are passed through an automatic redactor
that strips account-number and card-number fragments, Social Security
numbers, and similar sensitive sub-strings before the description is
stored. The redacted form is what you see in the app. (An account may
be configured to retain the full, un-redacted description for your
own record-keeping; this is off by default.)

### 2.3 Categorization data

Transactions arrive from Plaid with a suggested category. Mizu
presents that suggestion for you to confirm or correct, and stores
your confirmations and corrections with your account so your data
stays organized the way you want. No transaction data is sent to any
third-party artificial-intelligence or categorization service;
categorization uses Plaid's own category together with your input.

### 2.4 Push notifications

If you enable push notifications, we store an Apple Push Notification
service (APNs) device token provided by iOS. This token identifies
your device for the purpose of delivering notifications and contains
no personal data on its own. You can disable notifications at any
time from within the app or from your device settings, and we
automatically remove tokens that iOS reports as no longer valid.

### 2.5 Purchases

If you subscribe, your payment is handled by Apple's In-App Purchase
system — we never receive your card or payment details. We store a
record linked to your account so we can tell whether your
subscription is active: the Apple transaction identifier(s), the
product, the store environment, and the expiration date. This record
is deleted when you delete your account.

### 2.6 Basic usage and diagnostic data

Our servers keep operational logs — app version, server-side error
traces (no personal content), and authorization timestamps — for
reliability and abuse investigation. We do **not** embed any
device-side diagnostics, crash-reporting, advertising, marketing, or
behavioral-analytics SDK in the app; the app collects no telemetry
from your device. (On iOS, only Apple's own opt-in crash reporting
may share crash data with us, which is handled entirely by Apple.)

## 3. How We Use Information

We use the information described above to operate Mizu: to display
your financial data back to you, to help you confirm and correct
categorizations, to deliver notifications you have opted into, to
provide subscriber features to active subscribers, and to investigate
abuse or fraud.

We do not sell or rent personal information. We do not share personal
information with third parties for their independent marketing or
advertising purposes.

## 4. Sub-processors

We use the following sub-processors to operate Mizu. Each has been
reviewed for security posture and is bound by a written agreement
appropriate to the data we share with them.

| Sub-processor | Purpose | Data shared |
|---|---|---|
| Plaid Inc. | Bank-data aggregation | Bank account identifiers; the transaction stream is fetched on your behalf |
| Apple Inc. (Sign in with Apple) | Identity authentication (when you choose it) | Name and email, or an Apple private-relay email if you choose Hide My Email |
| Apple Inc. (App Store / In-App Purchase) | Subscription billing | Apple transaction identifiers and subscription status — never your card or payment details |
| Apple Inc. (Apple Push Notification service) | Push notifications (when enabled) | Opaque APNs device token |
| Supabase, Inc. | Database, authentication, and scheduled server functions | Your Mizu application data |

## 5. Storage and Security

Your Mizu data is stored in Supabase Postgres with row-level security
policies that isolate each user's records. Bank-aggregator access
tokens are encrypted with AES-256-GCM before storage; the encryption
key is held only on the application server and never leaves it. All
traffic between you, Mizu, and our sub-processors uses TLS 1.2 or
higher.

We undergo periodic security review and run automated security
advisor scans against our database.

## 6. Retention and Deletion

We retain your data for as long as your account is active. You can
permanently delete your account from Mizu's Settings; this:

- Disconnects any active bank connections, including removing them at
  Plaid.
- Deletes all of your transactions, labels, categories, notification
  tokens, purchase records, and other application data immediately.
- Removes your authentication record.

After deletion we retain a minimal deletion record — your email and
the deletion timestamp — as a record that the deletion occurred (for
fraud-prevention and to honor any re-signup limits). No transaction
data, labels, or other personal content is retained.

If you would like us to delete this minimal record as well, contact
us — see Section 8.

## 7. Your Rights

You may:

- **Access** all personal information we hold about you by signing
  into the app.
- **Export** all your data in JSON/CSV from Mizu's Settings.
- **Correct or update** any information by editing it in the app.
- **Delete** your account and associated data from Mizu's Settings.
- **Withdraw push notification consent** from the app's Notifications
  settings or your device's OS-level settings.

If you reside in a jurisdiction with additional privacy rights
(California, the European Union, the United Kingdom, and similar),
those rights also apply and you may exercise them by emailing us.

### 7.1 California Privacy Rights (CCPA / CPRA)

If you are a California resident, in addition to the rights above, the
California Consumer Privacy Act (as amended by the California Privacy
Rights Act) gives you the following rights with respect to personal
information we have collected about you:

- **Right to know** — request a copy of the categories and specific
  pieces of personal information we have collected about you, the
  sources of that information, the purposes for which we collected it,
  and the categories of third parties (sub-processors, listed in
  Section 4) with whom we have shared it.
- **Right to delete** — request that we delete the personal
  information we have collected from you. You can exercise this
  directly from Mizu's Settings (see Section 6).
- **Right to correct** — request that we correct inaccurate personal
  information. You can edit your data directly inside the app.
- **Right to opt out of sale or sharing** — we do not sell your
  personal information and we do not share it for cross-context
  behavioral advertising. There is therefore no "Do Not Sell or Share
  My Personal Information" link to display; the opt-out is our default
  for all users.
- **Right to limit use of sensitive personal information** — financial
  transaction data is considered sensitive personal information under
  CPRA. We use it only to provide the features you have signed up for
  (transaction labeling and exports). We do not use it to infer
  characteristics about you for any other purpose, and you may request
  that we further limit its use by emailing us.
- **Right to non-discrimination** — exercising any of these rights
  will not result in denial of service, different prices, or a
  different level or quality of service.

To exercise any of these rights, email **privacy@dmclabs.one** with
the request type and the email address associated with your account.
We will respond within 45 days. Where required, we will verify your
identity before fulfilling a request — typically by confirming you
can sign in to the account you are asking about.

You may also designate an authorized agent to make a request on your
behalf; agent requests must include a written authorization signed by
you and verification of the agent's identity.

## 8. Contact

For any privacy question, request, or concern, reach us at
**privacy@dmclabs.one** or via **https://www.dmclabs.one/contact**.

DMC Labs, LLC
Florida, United States

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. We will update
the version and date at the top of this document. For material changes
affecting your data rights, signed-in users will see an in-app
re-acceptance prompt before continuing.
