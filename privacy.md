# Privacy Policy

**Clinic Accounting Plugin**
Last updated: 12 June 2026

## 1. What this Software does
The Clinic Accounting Plugin is a privately deployed accounting automation tool for
medical clinics. It processes the engaging clinic's business documents (supplier
invoices, receipts, petty cash sheets, bank statements, and day-end sales exports) and
records accounting entries in the clinic's own QuickBooks Online company via Intuit's
official API.

## 2. Data we process
- Business/accounting documents uploaded or dropped into watched folders by the clinic.
- Master data entered by the clinic (chart of accounts, suppliers, procedures, staff
  payroll data, receivable customers).
- QuickBooks Online data necessary for the integration (chart of accounts, posted
  entries, vendor records), accessed via OAuth 2.0 authorization granted by the clinic.

The Software processes business financial data. It is not designed to collect patient
medical records; day-end sales exports contain service and payment information, not
clinical records.

## 3. Where data is stored
Data is stored in a database on infrastructure controlled by the clinic or its engaged
accountant (typically a local or self-hosted deployment). QuickBooks data remains in the
clinic's own QuickBooks Online account, governed by Intuit's terms and privacy policy.

## 4. Third-party services
- **Intuit QuickBooks Online** — accounting entries are posted to the clinic's own
  QuickBooks company via the official API. OAuth tokens are stored encrypted at rest.
- **Anthropic Claude API** — document text/images may be sent to Anthropic's API for
  data extraction (e.g. reading an invoice's supplier, amounts, and VAT). Extraction
  output is reviewed by a human before posting.

## 5. Data sharing
Data is not sold or shared with any party other than the services listed above, which
are used solely to provide the Software's functionality to the clinic.

## 6. Security
OAuth tokens are encrypted at rest. Access to the Software is authenticated and
role-based. The deployment is private to the engaging clinic and its accountant.

## 7. Data retention and deletion
Data is retained for the duration of the engagement and applicable statutory record
keeping periods. Upon termination, the clinic may request export and/or deletion of its
data from the deployment.

## 8. Disconnecting QuickBooks
The clinic may revoke the QuickBooks connection at any time from within the Software or
via Intuit's connected-apps settings (https://appcenter.intuit.com).

## 9. Contact
For privacy questions, contact the developer via the repository's issue tracker or the
contact details provided in your service agreement.
