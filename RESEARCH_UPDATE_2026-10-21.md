# Research update — 21 October 2026

**Five improvements to the research portfolio, using public primary evidence and original analysis.** Background investment reports shaped the questions and analytical sequence. Their conclusions, proprietary tables, charts and universes are not the evidence base for these new cases. AI assisted retrieval, analysis, drafting, coding and checking; independent human validation and workflow research approval are not claimed.

## 1. Add substantive cases inside existing repositories

| Case | Independent analytical finding | Deliverable |
|---|---|---|
| AI power / battery storage | A global cost benchmark becomes a site hurdle: reserve and maintained capacity have costs; backup benefits must be evidenced separately. | [Memo, chart, sources and model](https://github.com/HHFinAi/Sustainability-to-Financial-Materiality-Analysis/tree/main/examples/battery-storage) |
| Climate / staples earnings | Common shocks do not identify issuer exposures. Danone's cost reclassification changes a COGS-based sensitivity without changing baseline profit. | [Three-issuer case](https://github.com/HHFinAi/Sustainability-to-Financial-Materiality-Analysis/tree/main/examples/climate-staples) · [Climate handoff](https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets/tree/main/examples/climate-staples) |
| Water / waste operating monitor | Order concentration, group/segment growth, pricing and unusual volume comparators carry different information. | [Three-issuer monitor](https://github.com/HHFinAi/Sustainability-to-Financial-Materiality-Analysis/tree/main/examples/water-waste) |
| Brazil agriculture / nature | The current first-survey forecast is area-led. Productivity gains do not guarantee producer profits or observed land sparing. | [Public forecast decomposition and farm sensitivity](https://github.com/HHFinAi/Nature-and-Biodiversity-Investment-Agent/tree/main/examples/brazil-agriculture) |
| Ageing / sovereign finance | Demography is not a fiscal model. Productivity's effect on a benefit burden depends on indexation and employment. | [Three-country evidence and policy identity](https://github.com/HHFinAi/Sovereign-and-Social-Impact-Finance-Agent/tree/main/examples/ageing-fiscal) |

These are completed bounded research artifacts, not completed security underwriting. No new standalone agent or unsupported large company dataset was added. Existing cases and their historical conclusions are preserved.

## 2. Make each case independently inspectable

Each folder contains a concise memo, original visible chart, public-source register with dates/locators/units, explicitly labelled assumptions, offline Python model, archived JSON/Markdown results, sensitivities or discriminating comparisons, a contrary case and a next observation. Model reproduction uses Python 3.10+ without network access. Chart regeneration optionally uses Matplotlib.

Twenty-four new unit tests passed during preparation: 14 in financial materiality (including prospective scoring), five in nature and five in sovereign finance. They test break-even closure, physical/economic bounds, hedge/pricing timing, accounting presentation, decomposition, benefit indexation, missing outcomes and date/unit guards. Software checks are separate from source truth, human review and investment validity.

## 3. Close specific evidence gaps; retain the material unknowns

| Workstream | Gap addressed with public evidence | Still NEEDS_DATA before stronger claims |
|---|---|---|
| Storage | Updated IRENA four-hour installed-cost context; ATB efficiency/life/augmentation assumptions; explicit reserve/cost sensitivity. | Local bid, charging source, hourly dispatch, warranties, contracted availability and outage-loss economics. |
| Staples | Current H1 cost/margin structures and Danone's quantified presentation change; normalized lagged transmission model. | Procurement weights, regional crop exposure, hedge basis/expiry, FX, inventories, elasticity, perimeter and earnings/valuation bridge. |
| Water/waste | Primary Q2 releases; Xylem order-change concentration; separate Veralto group/segment growth; WM pricing and volume definitions. | Backlog conversion, cancellation terms, normalized cash/capital returns and valuation expectations. |
| Agriculture | Latest reviewed CONAB first-survey crop levels and growth rates; area/yield accounting and transparent price-cost break-even. | Consistent historical regional panel, realized harvests, farm economics, geospatial conversion, rights and issuer exposure. |
| Ageing | Consistent demographic definitions and separately sourced policy-conditional public-pension projections. | National benefit/employment rules, health/care costs, fiscal reactions, debt/currency/rate dynamics and security expectations. |

Public availability does not make projections observations, different accounting definitions comparable, or an agency aggregate an issuer exposure. The original AI/Brevik/EIB contractual and market-data gaps remain open; this update does not imply they have been resolved.

## 4. Add prospective evaluation

The [prospective register](https://github.com/HHFinAi/Sustainability-to-Financial-Materiality-Analysis/tree/main/evaluation/prospective-research) freezes three Q3 operating hypotheses before issuer-announced releases, with subjective probabilities, precise event definitions, first-release rules and a 50% naive benchmark. A deterministic scorer reports coverage and Brier scores only for dated, compatible observed outcomes. **At publication: three pending; zero scored; no accuracy or alpha claim.**

Prediction/source bytes are hashed; publication history supplies the chronological record. Hashes are not authenticated tamper-proof preregistration. Future observations and corrections must retain the original prediction and cutoff status. The manual review checkpoint is 30 November 2026; no scheduled service is implied. Existing extraction-evaluation results remain a separate record.

## 5. Curate the public profile around the research

The [profile](README.md) now leads with six research questions spanning AI power, climate earnings, water/waste, nature, sovereign finance and sustainable credit. Older Brevik, Microsoft, stewardship and integrated-portfolio work remains accessible. Repository landing pages point directly to new memos and models, with the climate repo linking the single canonical financial model.

This improves the evidence visitors can inspect. It does not establish increased traffic, stars, recruitment outcomes, investor adoption or performance; those would need subsequent measurement. GitHub's native pinned-repository settings were not changed by this documentation update.

[Standards](RESEARCH_STANDARDS.md) · [Open research gates](RESEARCH_ROADMAP.md) · [Capability catalogue](CATALOGUE.md)
