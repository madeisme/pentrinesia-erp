# ERP UMKM Documentation Index

This repository contains the working documentation for the Pentrinesia ERP PWA project.

## Project status

This project is still in the early design stage. The current direction is:

- one store, many users and devices
- owner, kasir, sales, and admin/gudang roles
- offline-first transaction flow
- home server on ZimaOS as the main system of record
- PostgreSQL as the preferred database candidate
- Tailscale as private remote access path
- Google Drive for offsite backup/export
- AI used for business strategy insight, not operational control

## Document set

### Product
- docs/product/vision-and-scope.md
- docs/product/roles-and-workflows.md
- docs/product/modules.md
- docs/product/reporting-and-tax.md

### Technical
- docs/technical/architecture.md
- docs/technical/offline-sync.md
- docs/technical/security.md
- docs/technical/backup-and-recovery.md
- docs/technical/zimaos-deployment.md

### Decisions
- docs/decisions/decision-log.md

## Product direction summary

This ERP is designed for a small UMKM with one store and multiple users and devices. It supports:

- sales and cashier workflow
- stock management and stock ownership separation
- price rules and promo logic
- customer and supplier records
- purchase and receivables/payables flow
- role-specific dashboards
- AI-based business recommendations without direct operational control

## Important design boundaries

- AI is not allowed to directly change prices, stock, transactions, or financial records.
- Operational data is the source of truth.
- Reporting and KPI are calculated by ERP logic, not by AI output.
- Offline transactions must be clearly marked and resolved safely.
- Backup and restore are required parts of the product foundation.

## Next steps

1. Review the product assumptions and role model.
2. Validate the pricing and stock ownership design.
3. Review the offline sync and conflict model.
4. Validate the backup and restore plan.
5. Convert the docs into a more formal repo-ready structure after team review.
