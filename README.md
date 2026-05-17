# Analytics Documentation Practice

*Ten documents, eighty-seven pages, one shared template. Three case studies in
how raw operational data becomes decision-ready output.*

---

This is a portfolio practice — not client work, not a paid engagement. Three
analytics projects, scrubbed of identifying details, packaged as if they
shipped to an internal team. The point is the documentation itself: how
findings get framed for executives, how dimensional models get explained
to engineers, how data quality decisions get audited, how runbooks survive
the 2 AM oncall page.

The work behind each project is mid-level analyst output. The documentation
discipline is what's being demonstrated.

## The three case studies

### → [01 · Marketplace SQL Analytics](./01-marketplace-sql-analytics/)

A Nigerian e-commerce platform: 865 customers, 90 sellers, 280 products,
3,015 orders. PostgreSQL cleaning, eight business queries, an executive memo,
a technical methodology report, a data quality audit, a query documentation
pack.

Headline finding: mid-rated products generate ₦141M more revenue than
high-rated products. High-rated products carry the lowest average unit price.
The intuitive read — that high ratings drive sales — is wrong at this
platform.

### → [02 · Distributor BI Dashboard](./02-distributor-bi-dashboard/)

A global gourmet food distributor: 830 orders, 89 customers, 21 countries,
22 months of data. Tableau dashboard with three pages, dashboard methodology
report, findings report with six findings and five recommendations.

Headline finding: revenue tripled in the final five months of the dataset,
order volume doubled in the same window. Both metrics moving together rules
out price as the driver. What caused it is not in the data.

### → [03 · Bank Warehouse Design](./03-bank-warehouse-design/)

A retail bank's transaction file, modeled into a PostgreSQL star schema.
Eight tables, SCD Type 2 on customer tier and branch name, surrogate keys
on every dimension, monthly aggregate table for reporting. Includes the full
dimensional model design, a column-level data dictionary, an ETL operations
runbook with troubleshooting playbook.

Headline decision: separating `dim_channel` and `dim_transaction_type` into
two dimensions instead of one. Combining them would force every analytical
question to pick a side.

## What's in each case study folder

Every case study folder follows the same structure: a brief `README.md` that
sets up the problem and points to the documents, a `/docs` folder with both
PDF and DOCX versions of every document, and a `/charts` folder with the
chart images used inside them. PDFs render in the browser. DOCX files
download for editing.

## On the documentation register

All ten documents share a single template — same cover layout, same TOC
generation, same heading hierarchy, same chart styling, same footer pattern.
They also share a writing register: direct prose, claims anchored to specific
numbers, limitations stated openly, no filler. Two anti-slop passes were
run across the bundle to catch the usual tells (Tier 1: *delve, leverage,
holistic*; Tier 3: *Furthermore, Moreover, It's worth noting*). Zero hits
across 2,142 paragraphs.

## On the scrubbing

Identifying details have been removed: real organization names, employee
names, customer names, and external URLs. The analytical work is faithful to
the source data; only the labels have been changed. This is a portfolio
artifact, not a client deliverable.

## Stack

PostgreSQL 18 · Python · Node.js (docx generation) · matplotlib (charts) ·
Tableau Public · LibreOffice (PDF rendering for validation)

---

*Pelumi Oladokun · Lagos, Nigeria · [https://pelumioladokun.xyz](https://pelumioladokun.xyz) ·
[oladokunpelumi07@gmail.com](mailto:oladokunpelumi07@gmail.com)*