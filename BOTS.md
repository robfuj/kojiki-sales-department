# Bots of Sales  (docx S5 candidate menu)

These are the **Major sub-functions** of Sales from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 10.

- `prospecting` — **Prospecting**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `account-research` — **Account Research**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `qualification` — **Qualification**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `opportunity-management` — **Opportunity Management**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `enterprise-sales` — **Enterprise Sales**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `account-management` — **Account Management**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `solutions-engineering` — **Solutions Engineering**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `sales-operations` — **Sales Operations**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `deal-desk` — **Deal Desk**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
- `sales-enablement` — **Sales Enablement**  ·  titles: CRO, Chief Sales Officer, VP Sales, Regional VP, Sales Director, Sales Manager, Account Executive, Enterprise AE, SDR/BDR, Sales Engineer
