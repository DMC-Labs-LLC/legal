---
version: "2026-06-22"
title: Privacy Policy
last_updated: June 22, 2026
---

# Privacy Policy

Last updated: June 22, 2026

## 1. Who We Are

DMC Labs, LLC ("DMC Labs," "we," "us," or "our") provides a family
of software applications including personal-finance tools, family
dashboards, and related services. This Privacy Policy applies to all
applications operated by DMC Labs and is referenced by each of them.

## 2. Information We Collect

### 2.1 Account information

When you sign in through a third-party authentication provider (such
as Google or Apple), we receive your name and email address. We do
not see your password. If you use Sign in with Apple, you may choose
Apple's Hide My Email option, in which case we receive only an
Apple-provided relay email address.

### 2.2 Financial transaction data

For finance applications (such as Mizu), we receive transaction data
from your bank through Teller, a regulated bank-data aggregator
acting on your behalf. We receive: account name, account type, the
last four digits of the account number, individual transaction date,
amount, merchant description, and posting metadata. We do **not**
receive your bank login credentials at any time. We do **not** have
the ability to move money — the connection is read-only.

Transaction descriptions are passed through an automatic redactor
that strips account-number and card-number fragments, Social Security
numbers, and similar sensitive sub-strings before the description is
stored and before it is used for AI labeling (see Section 2.3). The
redacted form is what you see in the app. (An account may be
configured to retain the full, un-redacted description for the
account holder's own record-keeping; this is off by default.)

### 2.3 Categorization data (AI labeling)

When you use the AI labeling feature (Mizu), the redacted transaction
description is sent to Microsoft Azure OpenAI to suggest a category
label. The request includes only the (redacted) description and the
list of candidate category names — no transaction amount, name,
email, account number, or other identifier is attached. Azure OpenAI
is configured to not retain or train on this content. We log each AI
labeling decision internally for reliability and auditing; you can
request a record of the AI labeling events associated with your
account by contacting us (see Section 9).

### 2.4 Child profile information (family applications)

For applications that include child dashboards (such as KiddoCash),
we collect: first name, color preference, and weekly allowance
settings the parent enters. Device identifiers and access timestamps
for authorized child devices.

### 2.5 Consent records

COPPA consent records include the parent's IP address at the time of
consent and the policy version they agreed to.

### 2.6 Push notifications

If you enable push notifications (in supported applications), we
store an opaque endpoint identifier and two cryptographic keys
provided by your browser (Web Push) or an APNs device token
(provided by iOS). These tokens identify your device for the
purpose of delivering notifications and contain no personal data
on their own. You can disable notifications at any time from
within the app, and we automatically remove tokens that have been
revoked by your browser or by iOS.

### 2.7 Anonymous access requests

If you submit a "Request Access" form for an invite-only application,
we store the email address and name and message you provide, plus a
hashed (one-way) version of your IP address for spam filtering.

### 2.8 Basic usage and diagnostic data

Our servers keep operational logs — application version, server-side
error traces (no personal content), and authorization timestamps —
for reliability and abuse investigation. We do **not** embed any
device-side diagnostics, crash-reporting, advertising, marketing, or
behavioral-analytics SDK in the app; the app collects no telemetry
from your device. (On iOS, only Apple's own opt-in crash reporting
may share crash data with us, which is handled entirely by Apple.)

### 2.9 In-app purchases (tips)

Some applications (such as Mizu) let you leave an optional in-app
tip through Apple's In-App Purchase system. Apple processes the
payment — we never receive your card or payment details. We keep a
record that the tip occurred, linked to your account: the Apple
transaction identifier, the product, the amount, and the date. We
use this only to recognize supporters and to honor any future
benefit we may choose to extend to early supporters (for example,
continued access if a paid tier is ever introduced). This record is
deleted when you delete your account.

## 3. How We Use Information

We use the information described above to operate the application
you signed up for: to display your financial data back to you, to
suggest categorizations, to deliver notifications you have opted
into, to enforce the COPPA consent record for child profiles, to
respond to access requests, and to investigate abuse or fraud.

We do not sell or rent personal information. We do not share
personal information with third parties for their independent
marketing or advertising purposes.

## 4. Sub-processors

We use the following sub-processors to operate our services. Each
has been reviewed for security posture and is bound by a written
agreement appropriate to the data we share with them.

| Sub-processor | Purpose | Data shared |
|---|---|---|
| Google LLC | OAuth authentication (when you choose Google sign-in) | Name, email, profile photo URL |
| Apple Inc. (Sign in with Apple) | Identity authentication (when you choose Apple sign-in) | Name and email, or an Apple private-relay email if you choose Hide My Email |
| Supabase, Inc. | Database, authentication, scheduled jobs (Edge Functions) | All application data |
| Netlify, Inc. | Web application hosting and request handling | Application requests and responses |
| Teller Inc. | Bank-data aggregation (finance apps only) | Bank account identifiers; transaction stream is fetched on demand |
| Microsoft Corporation (Azure OpenAI) | AI category labeling (finance apps only) | Redacted transaction description only — no amount, no identifiers |
| Apple Inc. (Apple Push Notification service) | iOS native push notifications (when enabled) | Opaque APNs device token |
| Your browser's Web Push service (e.g. Apple, Google, Mozilla) | Delivery of web push notifications to an installed web app (when enabled) | Opaque push endpoint, determined by your browser — not chosen by us |
| Resend, Inc. | Transactional email (parental-consent verification only) | Email address |

When a child profile is created in a family application, the parent's
email is the only identifier we hold for that flow; child first names
are stored encrypted at rest and are never sent to any sub-processor
except Supabase (which stores them).

## 5. Storage and Security

All application data is stored in Supabase Postgres with row-level
security policies that isolate each user's records. Bank-aggregator
access tokens are encrypted with AES-256-GCM before storage; the
encryption key is held only on the application server and never
leaves it. All traffic between you, our application, and our
sub-processors uses TLS 1.2 or higher.

We undergo periodic security review and run automated security
advisor scans against our database schema.

## 6. Retention and Deletion

We retain your data for as long as your account is active. You can
permanently delete your account from within each application's
Settings; this:

- Revokes any active bank-aggregator connections (Teller).
- Deletes all of your transactions, labels, categories, push
  subscriptions, in-app tip records, and other application data
  immediately.
- Removes your authentication record.

After deletion we retain a minimal deletion record — your email and
the deletion timestamp — as a record that the deletion occurred (for
fraud-prevention and to honor any re-signup limits). No transaction
data, labels, or other personal content is retained. COPPA consent
audit records are retained as required by law in anonymized form (no
child first name or device identifier).

If you would like us to delete this minimal record as well, contact
us — see Section 9.

## 7. Your Rights

You may:

- **Access** all personal information we hold about you by signing
  into the application.
- **Export** all your data in JSON/CSV from the application's
  Settings.
- **Correct or update** any information by editing it in the
  application.
- **Delete** your account and associated data from the application's
  Settings.
- **Revoke consent** (for parental consent in family apps) and
  request immediate deletion of associated child profiles.
- **Withdraw push notification consent** from the application's
  Notifications settings or your device's OS-level settings.

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
  features you have signed up for (transaction labeling, exports,
  retirement-modeling input). We do not use it to infer
  characteristics about you for any other purpose, and you may
  request that we further limit its use by emailing us.
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
are invite-only for adult users.

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
