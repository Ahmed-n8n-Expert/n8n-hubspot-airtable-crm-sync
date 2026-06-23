# n8n-hubspot-airtable-crm-sync
Enterprise-grade CRM Automation built on n8n. Seamlessly synchronizes HubSpot Leads and Deals with Airtable for advanced business dashboards and real-time tracking.
# 🏢 Enterprise CRM Data Pipeline (HubSpot + Airtable Sync Engine)

A high-performance, enterprise-grade CRM integration workflow built using **n8n**. This system automates the bidirectional synchronization of Contacts, Companies, and Deals between **HubSpot** and **Airtable**, enabling sales teams to enjoy automated data entry and clean business intelligence dashboards.

## 🚀 Key Features

- **Real-Time Lead Sync:** Instantly creates or updates a record in Airtable whenever a new lead or contact is generated inside HubSpot (via Webhooks).
- **Deal & Pipeline Tracking:** Automatically updates Airtable sales dashboards when a Deal stage changes in HubSpot (e.g., from "Proposal" to "Closed Won").
- **Smart Data Deduplication:** Uses conditional routing to search for existing Email/Record IDs before creating entries, ensuring completely clean databases with zero duplicates.
- **Two-Way Status Updates:** Allows custom data modifications made in Airtable by project managers to sync right back into HubSpot's timeline.

## 🛠️ Built With

- **n8n** (Enterprise Workflow Automation & Error Handling)
- **HubSpot API** (OAuth2 Integration / CRM Data Model)
- **Airtable API** (Relational Databases & Custom Views)
- **Custom JavaScript Node** (For formatting data types and telephone phone numbers)

## 📦 How to Deploy This Workflow

1. **Import to n8n:** Download the `hubspot-airtable-sync.json` file from this repository and upload it into your n8n workspace.
2. **Configure HubSpot OAuth2:** Set up your HubSpot developer credentials or access tokens inside the HubSpot node.
3. **Map Airtable Fields:** Connect your Airtable Base and Table. Ensure the field names in Airtable match the incoming data properties from HubSpot.
4. **Deploy Webhooks:** Activate the workflow to allow HubSpot's custom event triggers to instantly push data to n8n.

---
*Developed by Ahmed Tamer - AI Automation Engineer*
