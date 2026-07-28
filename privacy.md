---
version: "2026-07-28"
title: Privacy Policy
last_updated: July 28, 2026
---

# Privacy Policy

Last updated: July 28, 2026

## 1. Who We Are

DMC Labs, LLC ("DMC Labs," "we," "us," or "our") provides a family
of software applications including personal-finance tools, family
dashboards, and related services. This Privacy Policy applies to all
applications operated by DMC Labs and is referenced by each of them.

## 2. Information We Collect

### 2.1 Account information

When you sign in with Sign in with Apple, we receive your name and
email address from Apple. If you choose Apple's Hide My Email
option, we receive only an Apple-provided relay email address. If
you sign in with an email address and password, we store the email
address and a secure hash of the password (we cannot read the
password itself).

Your DMC Labs account is one identity across DMC Labs applications:
signing in to another DMC Labs application with the same account
gives that application access to the same data described in this
policy.

### 2.2 Financial transaction data

For finance applications (such as Mizu), we receive account and
transaction data from your bank through Plaid Inc. ("Plaid"), a
regulated bank-data network acting on your behalf. We receive:
account name, account type and subtype, the last four digits of the
account number, and for each transaction the date, amount, currency,
merchant name and description, merchant logo and website where
available, Plaid's category enrichment, and pending/posted status.
We do **not** receive your bank login credentials at any time —
bank sign-in happens on Plaid's interface. We do **not** have the
ability to move money; the connection is read-only.

Plaid's handling of your data is governed by Plaid's
[End User Privacy Policy](https://plaid.com/legal/#end-user-privacy-policy).

Bank connections are made at the level of your DMC Labs account,
not an individual application: a financial institution you link is
available to other DMC Labs applications you sign in to with the
same account. Your financial data is made available to **another
person's** account only if you explicitly grant that person access
to a specific linked account; you can revoke such a grant at any
time, and grants are recorded and auditable.

### 2.3 Categorization data

Finance applications help you confirm or correct the category of
each transaction. We store your review decisions and corrections,
and per-merchant preferences learned from your corrections, in
order to apply your choices to future transactions. Category
suggestions come from our bank-data provider's enrichment and from
your own corrections; no transaction content is sent to any
third-party artificial-intelligence service.

### 2.4 Child profile information (family applications)

For applications that include child dashboards (such as KiddoCash),
we collect: first name, color preference, and weekly allowance
settings the parent enters. Device identifiers and access timestamps
for authorized child devices.

### 2.5 Consent records

COPPA consent records include the parent's IP address at the time of
consent and the policy version they agreed to.

### 2.6 Push notifications

If you enable push notifications, we store the APNs device token
provided by iOS. This token identifies your device for the purpose
of delivering notifications and contains no personal data on its
own. You can disable notifications at any time from within the app
or in iOS Settings, and we automatically remove tokens that have
been revoked by iOS.

### 2.7 Basic usage and diagnostic data

Our servers keep operational logs — application version, server-side
error traces (no personal content), and authorization timestamps —
for reliability and abuse investigation. We do **not** embed any
device-side diagnostics, crash-reporting, advertising, marketing, or
behavioral-analytics SDK in the app; the app collects no telemetry
from your device. (On iOS, only Apple's own opt-in crash reporting
may share crash data with us, which is handled entirely by Apple.)

### 2.8 Purchases (subscriptions and tips)

Payments are processed by Apple's In-App Purchase system — we never
receive your card or payment details. For a subscription, we verify
the purchase directly with Apple and store: the Apple transaction
identifiers, the product purchased, and the subscription's current
expiration date, linked to your account. We keep a history of these
verification events for reliability and auditing. For an optional
tip, we store the Apple transaction identifier, the product, the
amount, and the date. These records are deleted when you delete
your account.

## 3. How We Use Information

We use the information described above to operate the application
you signed up for: to display your financial data back to you, to
apply your categorization choices, to determine your subscription
status, to deliver notifications you have opted into, to enforce
the COPPA consent record for child profiles, and to investigate
abuse or fraud.

We do not sell or rent personal information. We do not share
personal information with third parties for their independent
marketing or advertising purposes.

## 4. Sub-processors

We use the following sub-processors to operate our services. Each
has been reviewed for security posture and is bound by a written
agreement appropriate to the data we share with them.

| Sub-processor | Purpose | Data shared |
|---|---|---|
| Apple Inc. (Sign in with Apple) | Identity authentication | Name and email, or an Apple private-relay email if you choose Hide My Email |
| Apple Inc. (App Store / In-App Purchase) | Subscription and tip payment processing and verification | Purchase transaction identifiers |
| Apple Inc. (Apple Push Notification service) | iOS push notifications (when enabled) | Opaque APNs device token |
| Plaid Inc. | Bank-data network: institution linking and transaction retrieval (finance apps only) | Bank account connection on your behalf; see Plaid's End User Privacy Policy |
| Supabase, Inc. | Database, authentication, and server functions | All application data |
| Resend, Inc. | Transactional email (parental-consent verification only, family applications) | Email address |

When a child profile is created in a family application, the parent's
email is the only identifier we hold for that flow; child first names
are stored encrypted at rest and are never sent to any sub-processor
except Supabase (which stores them).

## 5. Storage and Security

All application data is stored in Supabase Postgres with row-level
security policies that isolate each user's records. Plaid access
tokens are encrypted with AES-256-GCM before storage; the
encryption key is held only in our server environment and is never
exposed to applications or users. All traffic between you, our
services, and our sub-processors uses TLS 1.2 or higher.

We undergo periodic security review and run automated security
advisor scans against our database schema.

## 6. Retention and Deletion

We retain your data for as long as your account is active. You can
permanently delete your account from within each application's
Settings; this:

- Removes your bank connections and deletes the associated access
  tokens from our systems.
- Deletes all of your transactions, categorization decisions,
  subscription and tip records, push registrations, and other
  application data immediately.
- Removes your authentication record.

After deletion we retain a minimal deletion record — your email and
the deletion timestamp — as a record that the deletion occurred (for
fraud-prevention and to honor any re-signup limits). No transaction
data, categorizations, or other personal content is retained. COPPA
consent audit records are retained as required by law in anonymized
form (no child first name or device identifier).

If you would like us to delete this minimal record as well, contact
us — see Section 9.

## 7. Your Rights

You may:

- **Access** all personal information we hold about you by signing
  into the application.
- **Export** your transaction data from the application's Settings.
- **Correct or update** any information by editing it in the
  application.
- **Delete** your account and associated data from the application's
  Settings.
- **Revoke consent** (for parental consent in family apps) and
  request immediate deletion of associated child profiles.
- **Revoke a sharing grant** you have made to another person's
  account at any time.
- **Withdraw push notification consent** from the application's
  settings or your device's OS-level settings.

If you reside in a jurisdiction with additional privacy rights
(California, the European Union, the United Kingdom, and similar),
those rights also apply and you may exercise them by emailing us.

### 7.1 California Privacy Rights (CCPA / CPRA)

If you are a California resident, in addition to the rights above,
the California Consumer Privacy Act (as amended by the California
Privacy Rights Act) gives you the following rights with respect to
personal information we have collected about you:

- **Right to know** — request a copy of the categories and specific
  pieces of personal information we have collected about you, the
  sources of that information, the purposes for which we collected
  it, and the categories of third parties (sub-processors, listed
  in Section 4) with whom we have shared it.
- **Right to delete** — request that we delete the personal
  information we have collected from you. You can exercise this
  directly from each application's Settings (see Section 6).
- **Right to correct** — request that we correct inaccurate personal
  information. You can edit your application data directly inside
  each application.
- **Right to opt out of sale or sharing** — we do not sell your
  personal information and we do not share it for cross-context
  behavioral advertising. There is therefore no "Do Not Sell or
  Share My Personal Information" link to display; the opt-out is
  our default for all users.
- **Right to limit use of sensitive personal information** —
  financial transaction data is considered sensitive personal
  information under CPRA. We use it only to provide the application
  features you have signed up for (displaying and categorizing your
  transactions, summaries of your own spending, and exports). We do
  not use it to infer characteristics about you for any other
  purpose, and you may request that we further limit its use by
  emailing us.
- **Right to non-discrimination** — exercising any of these rights
  will not result in denial of service, different prices, or a
  different level or quality of service.

To exercise any of these rights, email **privacy@dmclabs.one** with
the request type and the email address associated with your
account. We will respond within 45 days. Where required, we will
verify your identity before fulfilling a request — typically by
confirming you can sign in to the account you are asking about.

You may also designate an authorized agent to make a request on
your behalf; agent requests must include a written authorization
signed by you and verification of the agent's identity.

## 8. Children

Family applications such as KiddoCash include features designed for
use by children under the supervision of a parent or guardian. We
comply with the Children's Online Privacy Protection Act (COPPA):

- We never collect personal information from a child without verified
  parental consent.
- We collect only the child's first name and color preference — no
  email, no last name, no photographs.
- A parent can review, modify, and delete child information at any
  time from the parent's account.
- A parent can revoke consent at any time.

Finance applications such as Mizu are not directed at children and
require users to be 18 or older.

## 9. Contact

For any privacy question, request, or concern, reach us at
**privacy@dmclabs.one** or via **https://www.dmclabs.one/contact**.

DMC Labs, LLC
Florida, United States

## 10. Changes to This Policy

We may update this Privacy Policy from time to time. We will update
the version and date at the top of this document. For material
changes affecting your data rights, signed-in users will see an
in-application re-acceptance prompt before continuing.
