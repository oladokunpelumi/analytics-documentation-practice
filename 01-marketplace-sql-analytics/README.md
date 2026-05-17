# Marketplace SQL Analytics

*A Nigerian e-commerce platform. Eight business questions. Four documents.
Sixty-nine pages.*

---

## The problem

The platform — a marketplace selling electronics, fashion, beauty, home goods,
and four other categories — had two years of transactional data and no
analytical layer. Eight business questions sat unanswered: customer
acquisition by state, product revenue rankings, seller fulfilment efficiency,
quarterly trends, customer spend segmentation, payment preferences,
review/sales correlation, top-seller bonus qualification.

## The data

Seven tables, 13,755 rows total. 865 customers, 90 sellers, 280 products,
3,015 orders, 6,426 order items, 2,262 payments, 817 reviews. PostgreSQL 18.

## The four documents

1. **Executive Memo** — findings and recommendations for leadership. 11 pages.
2. **Technical Methodology Report** — every cleaning decision, every query
   pattern, why it was made. 19 pages.
3. **Data Quality Audit Report** — seven issues catalogued, all resolved,
   residual risk register. 15 pages.
4. **Query Documentation Pack** — Q1 through Q8, business question to logic
   to sample output to annotated SQL. 24 pages.

## What's surprising in the findings

Mid-rated products (3.0–3.99 stars) generate ₦498.6M in revenue. High-rated
products (≥ 4.0 stars) generate ₦357.5M. The mid-rated tier carries the
larger revenue, and the high-rated tier carries the *lowest* average unit
price (₦46,400). Customers may be rating cheaper, simpler products favourably
while spending on more expensive mid-rated SKUs. The Recommendation 1
intervention follows from that read.

## Read

- [Executive Memo (PDF)](./docs/01_executive_memo.pdf) — read this first.
- [Technical Methodology Report (PDF)](./docs/02_technical_methodology.pdf) —
  read this if you want the cleaning logic.
- [Data Quality Audit (PDF)](./docs/03_data_quality_audit.pdf) — read this
  for the audit trail.
- [Query Documentation Pack (PDF)](./docs/04_query_documentation_pack.pdf) —
  read this for the SQL.