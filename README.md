*Intuz — Your automation partner, one workflow at a time.*

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

[Intuz](https://www.intuz.com) helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[N8N Creator](https://n8n.io/creators/intuz/) · [AI Automation Company](https://www.intuz.com/company/) · [AI Chatbot Development](https://www.intuz.com/ai-agents-for-business-automation/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

# Automate expense reporting from Airtable to QuickBooks

This n8n template from Intuz provides a complete solution to automate your expense approval and accounting process.

It seamlessly connects an Airtable base, where expenses are submitted, to your QuickBooks account, eliminating manual data entry and ensuring financial records are always up-to-date.

## Who’s this workflow for?

- Accountants & Bookkeepers
- Small Business Owners
- Finance Teams
- Operations Managers

## How it works

1. **Trigger on New Expense:** The workflow starts automatically when a new expense record is added to your Airtable base.

2. **Filter for Approval:** It checks if the expense’s Status field is marked as “Approved”. Unapproved items are ignored.

3. **Create Expense in QuickBooks:** For every approved item, the workflow creates a new expense record in QuickBooks, mapping data like amount, date, vendor, and accounts directly from Airtable.

4. **Download and Upload Receipt:** It downloads the receipt from the URL provided in Airtable and uploads it as an attachment to the corresponding expense record in QuickBooks.

5. **Update Airtable Status:** Once the expense and receipt are successfully logged in QuickBooks, the workflow updates the record’s Status in Airtable to “Done”, closing the loop.

## Setup Instructions

### 1. Airtable Configuration

- Create an Airtable base with a table for your expenses. Ensure your table includes the following columns: Status, Receipt URL, Amount, Date, Memo, QBO Vendor ID, QBO Expense Account ID, and QBO Payment Account ID.
- Connect your Airtable account to n8n.
- In the Airtable Trigger, Search records, and Update record nodes, select your credentials and specify your Base ID and Table ID.

### 2. QuickBooks Configuration

- Connect your QuickBooks account to n8n using OAuth2 credentials.
- In the QBO-Create Expense and QBO-Upload File nodes, replace `{YOUR_QUICKBOOKS_COMPANY_ID}` in the URL with your actual QuickBooks Company ID.
- Ensure the Vendor ID and Account IDs in your Airtable records correspond to valid IDs in your QuickBooks account.

### 3. Activate Workflow

Save the workflow and toggle the **Active** switch to ON. Your expense management is now fully automated!

## FAQ

**Is this template free to use?**
Yes. It's an open-source n8n workflow published by Intuz — copy the workflow JSON from this repo and import it into your own n8n instance at no cost.

**Do I need a paid n8n plan to run this?**
No. It runs on n8n's free self-hosted Community Edition or on n8n Cloud. You'll need your own credentials for the services this workflow connects to, not a specific n8n pricing tier.

**What happens to expenses that aren’t approved yet?**
They are ignored. The workflow only processes records where Status is set to “Approved.” Once logged in QuickBooks, the Airtable status is updated to “Done.”

## Related n8n templates from Intuz

- [Automate full-cycle invoicing from Airtable to QuickBooks and Stripe](https://github.com/Intuz-production/QuickBooks-Invoice-Payment-Automation)
- [Automate QuickBooks customers & sales receipts generation from a Google Sheet](https://github.com/Intuz-production/Automate-QuickBooks-Customer-Sales-Receipt-Creation)
- [Automate real-time QuickBooks invoice sync to Google Sheets](https://github.com/Intuz-production/QuickBooks-Invoice-Sync)

[See all of Intuz's free n8n templates](https://www.intuz.com/n8n-workflow-automation-templates/)

## Connect with us

Intuz is a USA-based AI & workflow automation company with 16+ years of experience building custom AI-enabled workflow automations for SMBs and Enterprises, specializing in agentic AI, LLM integrations, and CRM/ERP sync across Healthcare, FinTech, eCommerce, Manufacturing, and Real Estate.

* **Website:** [https://www.intuz.com](https://www.intuz.com)
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz/
* **Get Started:** https://n8n.partnerlinks.io/intuz/

## For Custom Workflow Automation

[Click here - Get Started](https://www.intuz.com/get-started/)
