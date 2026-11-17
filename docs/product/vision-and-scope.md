# Vision and Scope

## 1. Product summary

Pentrinesia ERP is designed for a single-store UMKM with multiple users and devices. It aims to simplify daily store operations while still creating reliable financial, stock, and operational visibility for the owner.

The product combines:
- operational tracking
- financial overview
- inventory controls
- KPI reporting
- AI-based strategic insight

The system should be easy enough for a cashier to use every day, but detailed enough for owner and admin to monitor business health.

## 2. Target users

### Owner
The owner monitors the health of the business and needs quick visibility into:
- sales
- cash flow
- receivables and payables
- inventory risks
- margin pressure
- key product trends

### Kasir
Kasir works on daily transactions and needs a fast workflow:
- scan product
- add item to cart
- apply valid price or promo
- accept payment
- print or save receipt

### Sales
Sales works outside the store and needs access to customer data, product catalog, quotations, and price rules.

### Admin / Gudang
Admin or warehouse staff manages receiving, stock movement, stock adjustment, and stock opname.

## 3. Business goals

1. Make daily store operations simpler and faster.
2. Improve stock accuracy and reduce mismatch risk.
3. Separate own stock and consignment stock clearly.
4. Give owners visible financial and operational data.
5. Support multiple devices and users in a single store.
6. Provide AI insight for strategic recommendations without changing operational data.
7. Ensure safe backup and restore.

## 4. Product principles

### Operational first
The product must be usable for daily business operations before advanced AI or automation are added.

### Traceable data
Every important action and change must be traceable to who did it, when, and on which device.

### AI as strategy support, not operational control
AI should provide insight and suggestions such as:
- price pressure
- slow-moving stock
- bundling idea
- margin erosion
- late payment risk

AI must not directly:
- change product price
- alter stock balance
- edit transaction records
- modify tax settings
- create payment or accounting entries without review

### Offline-first and honest sync
The system should keep working while connectivity is unstable. It must clearly show local pending status, sync status, and conflict state.

## 5. Scope

### In scope for MVP
- product master data
- unit conversion
- pricing rules
- promo rules
- stock tracking
- stock ownership separation
- sales workflow
- purchase workflow
- customer and supplier data
- receivables and payables
- basic reports
- document generation and print
- role-based access
- offline sync queue
- backup and restore
- AI strategy insight

### Out of scope for MVP
- multi-store operations
- multi-company accounting
- deep tax automation without human review
- autonomous AI actions on core data
- complex warehouse management

## 6. Key business rules

### Own stock vs consignment stock
Stock ownership must be explicit and separate. Own stock and consignment stock must never be mixed in a single inventory balance without clear reporting context.

### Price rules
ERP must support multiple price sources:
- base product price
- customer group price
- quantity-based price
- special customer price
- promo price
- discount rules

### Promo rules
Promo must carry clear validity, scope, stacking rules, and approval policy.

### Tax handling
Tax configuration is a business tool, not a legal authority. It helps generate output and prepare data, but the user remains responsible for final review and compliance.

## 7. Success metrics

The product is successful when:
- kasir can process transactions quickly
- owner understands business health from dashboards
- sales can work on quotations and orders
- stock mismatches are easier to prevent
- backups are reliable and restore works
- AI recommendations are useful and reviewable

## 8. Open questions

- Should the cashier flow remain PWA-only or is a native Android app required?
- What exact pricing priority rules should be used when several rules overlap?
- How much offline functionality must be available for sales before MVP is considered usable?
- What are the reporting and tax outputs required by the business?
