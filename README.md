# Open-source Infrastructure Overview

This repository contains the setup and configuration of several open-source platforms used for internal business operations, monitoring, and automation.

## 📁 Systems Breakdown

### 1. `airbyte`
**Purpose:** Data integration (ETL/ELT) platform to sync data from various sources (e.g. databases, APIs) into destinations like PostgreSQL or data warehouses.

---

### 2. `authentik`
**Purpose:** Identity Provider for authentication, SSO, and access control for internal services.

---

### 3. `gitingest-main`
**Purpose:** Custom or internal service to automate Git-based ingestion workflows or triggers. May integrate with Jenkins or data pipelines.

---

### 4. `grafana`
**Purpose:** Visualization and monitoring tool. Used to display dashboards for Prometheus and other data sources.

---

### 5. `horilla`
**Purpose:** Internal platform or service (CRM / HRM / Workflow system depending on customization).

---

### 6. `jenkins`
**Purpose:** CI/CD automation platform to run build, test, and deployment pipelines.

---

### 7. `metabase`
**Purpose:** Business intelligence (BI) and data exploration tool. Simple SQL-based dashboards and analytics.

---

### 8. `odoo`
**Purpose:** ERP system covering multiple business modules like CRM, sales, accounting, inventory, etc.

---

### 9. `prometheus`
**Purpose:** Time-series metrics collection tool. Collects performance metrics from services to be used in Grafana.

---

### 10. `superset`
**Purpose:** Powerful data exploration and dashboard tool, supports SQL-based analytics.

---

### 11. `vtigercrm`
**Purpose:** Open-source CRM system to manage contacts, sales pipelines, and customer relations.

---

### 12. `wiki`
**Purpose:** Internal documentation (likely using Wiki.js or BookStack). Used to centralize team knowledge.

---

## 🔧 Integrations & Workflow

- **CI/CD:** GitHub + Jenkins pipelines are used for continuous deployment.
- **Monitoring:** Prometheus + Grafana stack is used to monitor system metrics.
- **Data:** Airbyte syncs data sources; Metabase and Superset visualize them.
- **Access Control:** Authentik handles SSO and login management.
- **ERP & CRM:** Odoo and Vtiger handle business and customer processes.
- **Documentation:** Wiki system is used for internal team knowledge base.

---

## 📌 Notes

- All services are containerized via Docker.
- Services are protected behind reverse proxy with proper SSL.
- SSO via Authentik is integrated into most dashboards for unified access.

---

