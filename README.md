# FIRAT CEM GURBEY

**Software Developer**

REDACTED@mail.com · REDACTED · [linkedin.com/in/cemgurbey](https://www.linkedin.com/in/cemgurbey) · [github.com/cemgurbey](https://github.com/cemgurbey)

> The compiled PDF version is **[resume.pdf](resume.pdf)** — it is rebuilt automatically by GitHub Actions on every push, so it always matches `resume.tex`.

---

## Education

**McGill University** — Sept. 2017 to May 2022
B.Sc. Computer Science, Minor in French

## Skills

**PROGRAMMING LANGUAGES:** Python, C/C++, Ruby, JavaScript
**TECHNOLOGIES:** Claude, MCP, Linux, Bash, Git, SQL, NoSQL, REST, GraphQL, HTML/CSS, React, Rails, Django, Pandas, PyTorch, Google Cloud, AWS, Docker
**LANGUAGES:** English, French, Turkish

## Employment

### ARC Group Benefits Inc. — Software Developer · Montréal, QC — Sept. 2023 to Present
- Led the migration of operational teams from waterfall-style project tracking to Asana by building a bidirectional Rails–Asana integration using the Asana API and webhooks, enabling agile workflows and automating downstream actions such as policy renewals and report generation
- Designed a concurrency-control mechanism to serialize webhook processing around Rails transactions, preventing race conditions and ensuring webhook-driven updates were queued and applied after record locks were released
- Shipped a Rails commission platform handling configurable, multi-party payout splits with per-recipient, per-category rate rules, including reconciliation logic when a third party withholds the full payment upfront and remits the remaining share separately, and cron-scheduled statement generation, replacing a manual process
- Served as engineering escalation point for 80+ production incidents and bugs, including recovery from a migration failure that wiped customer data, restoring from a prior state and verifying integrity via system logs
- Strengthened SOC 2 and security compliance by closing admin access-control gaps, restricting sensitive reports by role, automating contract-end account revocation, and eliminating user-enumeration and information-leakage vectors in UI
- Reviewed 300+ pull requests across nine engineers, catching defects before release and keeping conventions consistent

### Amazon Music — Software Development Engineer · Montréal, QC — June 2023 to Aug. 2023
- Ported Swift/Kotlin screens to React Native, consolidating iOS/Android into one codebase and reducing maintenance
- Built the customer onboarding interface with scrollable lists, carousels, and interactive navigation controls
- Connected components to GraphQL, rendering live account and catalogue data with loading and error states

### Shopify — Backend Developer · Montréal, QC — June 2022 to May 2023
- Built and scaled custom data (metafields and metaobjects) in Rails for Shopify's 1st- and 3rd-party apps, migrating endpoints from REST to GraphQL, replacing deprecated content permissions with metaobjects
- Reduced metaobject create/update latency by 10% through bulk operations; hardened the Metafield loader with fallbacks and resolved a Rails/MySQL string-encoding mismatch
- Implemented country-specific currency localization for money metafields in the Shopify's admin API and extended GraphQL schemas with new fields to eliminate redundant client-side queries
- Diagnosed cross-API inconsistencies through targeted debugging and contributed fixes across services; maintained Shopify's public API documentation with validated GraphQL query examples

### Matrox — Software Designer · Dorval, QC — Jan. 2022 to April 2022
- Worked on the development of the Mura IPX video capture cards on Windows and Linux platforms using C/C++
- Integrated the SRT protocol into Matrox's Vwlib library, cutting down the packet loss of streams to less than 1%
- Refactored the codebase of casting protocols in C++, delivering a clean interface for a complex subsystem
- Added timestamps on system outputs of the encoder/decoder to pinpoint behaviour changes during debugging

## Projects

### [Computer Vision Project](https://github.com/cemgurbey/plastic-water-segmentation) — Aug. 2026 to Present
- Built a machine learning model that detects plastic residue on water bodies using instance segmentation
- Generated synthetic training images with diffusion inpainting, replacing cut-and-paste composites
- Refined masks with SAM 2 and trained YOLO11 segmentation on native polygon labels in PyTorch
- Repackaged the workflow as a pip-installable CLI (synthesize, train, infer) with modern Python tooling

### [Sleep Log Analysis Tool](https://github.com/cemgurbey/sleep-log-data-analysis) — May 2022 to Sept. 2026
- Converted McGill's Attention, Behaviour and Sleep Laboratory's survey data into SPSS variables in Python
- Rebuilt the monolithic notebook as an installable package with CLI commands and typed modules
- Added a seeded synthetic data generator, so the pipeline runs end-to-end with example results
- Transposed horizontally-integrated data for faster processing using NumPy and pandas
