# EyeLex Privacy Policy

**Effective date:** 24 April 2026
**Last updated:** 24 April 2026

EyeLex (“we”, “us”, or “our”) is a legal-practice management mobile application
operated by **Fiscal Ox Private Limited** (“the Company”). This Privacy Policy
describes how we collect, use, store, and share your personal information when
you use the EyeLex mobile app (“the App”) and related services.

If you have questions, contact us at **support@fiscalox.com**. For grievance
redressal (required under India’s Digital Personal Data Protection Act, 2023),
write to our Grievance Officer at **support@fiscalox.com**.

---

## 1. Who this policy applies to

EyeLex is built for legal professionals — law firms, practising advocates, and
their clients who collaborate with them. It is not directed at children under 18.

---

## 2. Information we collect

We collect the following categories of personal information:

**Account information (always collected):**
- Name, email address, phone number
- Password (stored as a one-way hashed value; never retrievable by us)
- City, state, role (law firm / lawyer / client)
- Firm name, bar-council enrolment number, courts of practice, advocate code, cause-list name (for lawyers and firms)
- Authorised-representative name, CIN, PAN (for client accounts)
- Google account identifier, profile display name, and profile email when you sign in with Google

**Business and billing information (optional, entered by you):**
- Client records (names, contact details, addresses, PAN, CIN) that you add to the app
- Matter / case details (case numbers, court names, parties, opposing counsel, hearing dates, notes, status)
- Invoice data (amounts, tax, currency, payment status, timing)
- Bank account details you enter for invoice “Payment Instructions” (bank name, account holder name, account number, IFSC code, branch, UPI handle)

**Documents (optional, uploaded by you):**
- Files you attach to matters (contracts, annexures, scanned documents) are stored in our Amazon S3 bucket.

**Technical information (automatic):**
- Device model, operating system version, app version
- Crash reports and basic diagnostic logs (no personally identifying content)
- IP address at the time of each request (used for rate-limiting and abuse detection; not linked to individual user profiles)

We do **not** collect location data, contacts, camera media beyond files you explicitly attach, microphone input, or precise advertising identifiers.

---

## 3. How we use your information

We process the above data to:

- Create and maintain your EyeLex account.
- Authenticate you on every login (via email + password or Google Sign-In).
- Let you manage your clients, matters, court dates, invoices, and documents.
- Render invoice PDFs that include your firm’s bank payment instructions.
- Store matter documents securely in the cloud and make them retrievable only by you.
- Diagnose crashes and improve reliability.
- Comply with applicable legal obligations (e.g., tax record-keeping).

We do **not** use your data to train machine-learning models, sell it to advertisers, or share it with unaffiliated third parties for marketing.

---

## 4. How and where your data is stored

- **Application database** — Amazon RDS for PostgreSQL, hosted in the Mumbai (`ap-south-1`) AWS region.
- **File storage** — Amazon S3 bucket `eyelex-documents-1`, hosted in the same region.
- **Transit** — all traffic between the App and our backend uses TLS (HTTPS).
- **At-rest encryption** — select sensitive columns (tokens, credentials) are encrypted at the application level using AES-256-GCM. The underlying AWS services provide additional disk-level encryption.
- **Passwords** — stored only as one-way BCrypt hashes; we cannot see or recover your password.

---

## 5. Third-party services we rely on

We use the following third-party services. Each one only receives the data it strictly needs to perform its function:

| Service | Purpose | Data shared |
|---|---|---|
| **Google Sign-In** | Authenticate users who choose Google login | Email, name, Google account identifier |
| **Amazon Web Services** (RDS, S3, EC2) | Application hosting and data storage | All data covered by this policy |
| **Razorpay IFSC Directory** (`ifsc.razorpay.com`) | Validate IFSC codes entered during bank setup | The IFSC code only — no user identity leaves the app |

We do not integrate any advertising SDKs, analytics SDKs that collect personal data, or social-media login other than Google.

---

## 6. Who can see your data

Within the App, your data is visible only to you. Different firms and users are isolated: one lawyer’s matters are never shown to another user.

We may disclose data **only when legally required**:
- In response to a valid court order, summons, or lawful request from a law-enforcement authority having jurisdiction.
- To establish or exercise our legal rights or defend against legal claims.

We do not sell, rent, or commercially share your personal data.

---

## 7. Your rights

You have the right to:

- **Access** the personal information we hold about you.
- **Correct** inaccurate information — most fields are editable inside the App directly.
- **Delete** your account and all associated personal data. To request deletion, email **support@fiscalox.com** from the address registered with your account. We will process the request within 30 days.
- **Withdraw consent** to further processing, at which point we will either delete your account or anonymise it.
- **Lodge a grievance** with our Grievance Officer at **support@fiscalox.com**. Indian users may further escalate to the Data Protection Board of India.

---

## 8. Data retention

- We retain your account data for as long as your account is active.
- After account deletion, your records are purged within 30 days, except where longer retention is required by law (e.g., tax or billing records, which we may retain for up to 8 years as required under Indian tax regulations).
- Matter documents are deleted from S3 as part of account deletion.

---

## 9. Security

We follow industry-standard practices:
- HTTPS (TLS 1.2+) on all network traffic.
- One-way hashed passwords (BCrypt).
- AES-256-GCM encryption on sensitive application-level columns.
- Principle-of-least-privilege IAM roles for backend access to S3 and RDS.
- Regular security-patch upgrades to operating systems and runtimes.

No system is 100% secure. If you discover a security issue, please report it to **support@fiscalox.com**.

---

## 10. Children

EyeLex is intended for adult legal professionals and business clients. We do not knowingly collect personal data from children under 18. If you believe a child has provided us information, contact **support@fiscalox.com** and we will delete it.

---

## 11. Changes to this policy

We may update this policy periodically. Material changes will be announced inside the App and on this page. The “Last updated” date at the top reflects the most recent change. Continued use of the App after an update means you accept the revised policy.

---

## 12. Contact

For all privacy matters, contact:

**Fiscal Ox Private Limited**
Email: **support@fiscalox.com**
Grievance Officer: **Vicrumnaug Vuppalapaty**, **support@fiscalox.com**
Address: ** SWC HUB, 341, Vasna - Bhayli Main Rd, Bhayli, Vadodara, Gujarat 391410**

---

*This policy is provided for informational purposes and is not legal advice. If you need legal guidance specific to your business, consult a qualified practitioner.*
