---
version: "2026-02-16"
title: Privacy Policy
last_updated: February 16, 2026
---

# Privacy Policy

Last updated: February 16, 2026

## 1. Introduction

DMC Labs, LLC ("DMC Labs," "we," "us," or "our") respects your privacy. This Privacy Policy explains how we collect, use, and protect your personal information when you use our software applications and services.

## 2. Information We Collect

### Account Information

When you sign in through a third-party authentication provider (such as Google), we receive your name and email address.

### Financial Data

Certain applications allow you to upload financial transaction data (such as CSV bank statements) or connect financial accounts through third-party services. This data may include transaction dates, amounts, and descriptions. We automatically redact sensitive information (such as account numbers, card numbers, and Social Security numbers) from transaction descriptions at the time of upload.

### Child Information

When you create a child profile, we collect only the child's first name and a color theme preference. Children do not create their own accounts and cannot provide personal information directly. All child data is created and managed by the parent or guardian.

### Device Information

When a device accesses a child dashboard, we collect a randomly generated device identifier, the device type (derived from the browser's User-Agent string), and timestamps of access. This information is used solely to manage device authorization and is not shared with third parties.

### COPPA Consent Records

When you complete the parental consent process, we log consent events including timestamps, the version of our policies you accepted, your IP address, and a device identifier. These records are maintained for compliance purposes.

### Usage Data

We may collect basic usage information such as pages visited and features used to improve our services.

## 3. How We Use Your Information

We use your information to:

- Provide and maintain our services
- Authenticate your identity
- Display your financial data within our applications
- Manage device authorization for child dashboards
- Verify parental consent as required by COPPA
- Send transactional emails related to parental consent verification
- Improve and develop our services

We do not use your information for advertising, profiling, or marketing purposes.

## 4. Children's Privacy (COPPA Compliance)

We comply with the Children's Online Privacy Protection Act (COPPA). Our practices include:

**Verifiable Parental Consent.** Before any child profile can be created, we require verifiable parental consent using an email-based verification process. This process includes two steps separated by a mandatory waiting period to ensure the consenting party is the parent.

**Limited Data Collection.** We collect only a child's first name and color theme preference. Children cannot enter personal information, communicate with others, or make purchases through our services.

**Parental Controls.** Parents can at any time:

- View all data associated with their child's profile
- Export their child's data
- Delete their child's profile and all associated data
- Approve, revoke, or manage device access to their child's dashboard
- Revoke consent by deleting the child's profile or contacting us

**No Third-Party Sharing.** We do not share children's information with third parties. Bank account data accessed through third-party financial services (such as Teller) contains only the parent's financial information and is never associated with or accessible to children.

**Operator Information.** DMC Labs, LLC is the operator of these services. For questions about our children's privacy practices, contact us at [privacy@dmclabs.one](mailto:privacy@dmclabs.one).

## 5. Data Storage and Security

Your data is stored securely using Supabase, which provides encryption at rest and in transit. We implement row-level security policies to ensure that your data is only accessible to you.

Additional security measures include:

- **Token hashing:** Access tokens are stored as one-way hashes; plaintext tokens are never persisted
- **Device binding:** Child dashboards require explicit device authorization by the parent
- **PII redaction:** Sensitive information is automatically stripped from financial transaction descriptions
- **Inactivity controls:** Device access is automatically paused after 90 days of inactivity

We do not sell, rent, or share your personal data with third parties for marketing purposes.

## 6. Third-Party Services

Our applications may use the following third-party services:

- **Google** — Authentication (OAuth)
- **Supabase** — Database and authentication infrastructure
- **Vercel** — Application hosting
- **Resend** — Transactional email delivery (parental consent verification only)
- **Teller** (planned) — Bank account connectivity for financial data import

Each of these services has its own privacy policy governing how they handle your data. When connecting a bank account through Teller, you will be presented with a disclosure explaining what data is accessed and how it is used before any connection is established.

## 7. Cookies

We use cookies strictly for functional purposes:

- **Authentication cookies** managed by Supabase to maintain your login session
- **Device identification cookies** scoped to individual child dashboard paths, used to identify authorized devices

We do not use cookies for tracking, analytics, or advertising.

## 8. Data Portability

You may export your data at any time from the application settings in JSON or CSV format. Exports include your profile information, child profiles, transaction history, and allowance configurations.

## 9. Data Retention and Deletion

We retain your data for as long as your account is active. You may delete individual child profiles or your entire account at any time through the application settings.

**Child profile deletion** permanently removes the child's profile, all transaction history, allowance configurations, and device authorizations.

**Account deletion** permanently removes your parent profile, all child profiles, all associated data, and your authentication credentials. A record of the deletion event (timestamp and anonymized identifier) is retained for audit purposes.

Deletion is immediate and irreversible. We recommend exporting your data before deleting your account.

## 10. Your Rights

You have the right to:

- Access the personal information we hold about you
- Request correction of inaccurate data
- Request deletion of your data
- Export your data in a portable format
- Revoke parental consent for your child's data

These rights can be exercised directly through the application or by contacting us at the email address below.

## 11. Changes to This Policy

We may update this Privacy Policy from time to time. We will notify users of material changes by updating the "Last updated" date and requiring re-acceptance within our applications. Continued use of our services after changes constitutes acceptance of the revised policy.

## 12. Contact

If you have questions about this Privacy Policy, our children's privacy practices, or wish to exercise your data rights, please contact us at [privacy@dmclabs.one](mailto:privacy@dmclabs.one).
