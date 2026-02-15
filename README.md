# 🧱 Salesforce CI/CD & Release Management Simulation

## 📌 Overview
This project simulates an enterprise-grade Salesforce release management lifecycle using Salesforce CLI, Git branching, QA validation, and rollback engineering.

## 🏗 Environment Setup
- DevOrg (Development)
- QAOrg (Quality Assurance)
- CLI-based deployment workflow

## 🚀 Features Implemented
- Record-triggered Flow (Before-Save Optimization)
- Opportunity scoring automation
- Validation rule for stage control
- Permission set configuration

## 🔄 Release Lifecycle Simulated
1. Feature development in Dev
2. Metadata retrieval using Salesforce CLI
3. Git branching strategy (feature → develop → master)
4. QA dry-run validation
5. QA deployment & smoke testing
6. Incident simulation (logic regression)
7. Git-based rollback using `git revert`
8. Redeployment & validation

## 📄 Documentation
- QA-Validation-Results.md
- Incident-Rollback-Report.md

## 🎯 Key Learnings
- Difference between before-save and after-save flows
- Importance of CLI-based deployment validation
- Lightning page vs Page layout behavior
- Field-Level Security impact on deployment
- Professional rollback strategy using Git revert

---

This project demonstrates release discipline, governance awareness, and deployment stability practices beyond basic Salesforce administration.
