<!-- Profile redesign: original graphics and copy; layout inspired by github.com/flycran. -->
<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Sustainable Finance AI — climate investing, fundamental research and AI. Sources to scenarios to valuation to human judgment." />
</p>

<p align="center">
  <a href="https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets"><b>Explore the climate agent</b></a> &nbsp; · &nbsp;
  <a href="#research-workflows"><b>Workflows</b></a> &nbsp; · &nbsp;
  <a href="#selected-research-projects"><b>Research projects</b></a> &nbsp; · &nbsp;
  <a href="https://github.com/hh-health-AI"><b>Sector research</b></a>
</p>

<blockquote>
  <p align="center"><b>From climate and company evidence to explicit investment assumptions.</b><br />AI should improve research coverage without obscuring sources, uncertainty or accountability.</p>
</blockquote>

## About me

I build **AI-assisted research workflows, analyst skills and public-data tools** for sustainable investing and fundamental equity research. My focus is the connection between evidence, business economics, valuation and human investment judgment.

- **Research:** Climate investing, sustainable finance, growth equities and company earnings.
- **Methods:** Competitive analysis, cash-flow valuation, scenario analysis and evidence-based investment theses.
- **Workflow design:** Reusable agent instructions, structured handoffs, traceable research records and human review.

## Start here: Climate Investment AI Agent

<table>
<tr><td>
<h3><a href="https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets">Climate Investment AI Agent</a></h3>
<p><b>Connect climate risk to equity valuation and bond credit analysis.</b></p>
<p>A Python workflow engine with 20 specialist roles and seven instrument-aware routes, designed to organize climate research while keeping evidence references, assumptions, revisions and human review inspectable.</p>
<p><b>Core value:</b> Inspect the evidence and assumptions behind the conclusion—not just the generated narrative.</p>
<p><code>Evidence</code> → <code>Climate scenarios</code> → <code>Financial transmission</code> → <code>Equity / credit</code> → <code>Human review</code></p>
<p><a href="https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets/blob/main/docs/EVIDENCE_AUDIT.md"><b>Inspect the evidence layer →</b></a> &nbsp; · &nbsp; <a href="https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets#run-the-local-tests-and-synthetic-demo">Run the synthetic demo →</a></p>
</td></tr>
</table>

**Scope:** The engine orchestrates and validates research artifacts. An external AI host or human performs the research. There is no embedded LLM, live market feed, broker connection or autonomous trading. Reviewable records are not independent audit certification.

<!-- workflow-charts:start -->
## Research workflows

### Climate risk → equity valuation and bond credit

The [Climate Investment AI Agent](https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets#climate-risk-to-equity-valuation-and-bond-credit-analysis) connects mandate and evidence to climate analysis, instrument-specific underwriting, portfolio review and a human research decision.

```mermaid
flowchart TD
    M[Mandate and instrument scope] --> E[Evidence and entity boundaries]
    E --> S[Science and materiality]
    E --> D[Policy and disclosure context]
    E --> C[Emissions and targets]
    S --> P[Physical risk and adaptation]
    S --> T[Transition and opportunities]
    D --> T
    C --> T
    S --> Q[Scenarios and model risk]
    D --> Q
    P --> F[Financial transmission and double-counting check]
    T --> F
    Q --> F
    F --> EQ[Equity valuation]
    F --> CB[Corporate credit]
    F --> SB[Sovereign and municipal debt]
    F --> SC[Structured credit]
    F --> LB[Labelled-debt integrity]
    EQ --> PF[Portfolio and constraint review]
    CB --> PF
    SB --> PF
    SC --> PF
    LB --> PF
    PF --> ST[Stewardship and monitoring plans]
    ST --> RT[Independent challenge]
    RT --> IC[Investment memo]
    IC --> H[Human research decision]

    %% Profile presentation only; source workflow labels and connections are unchanged.
    classDef default fill:#ecfdf5,stroke:#059669,color:#052e16
    classDef decision fill:#065f46,stroke:#065f46,color:#ffffff
    class H decision
```

[**Explore the source workflow and implementation →**](https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets#climate-risk-to-equity-valuation-and-bond-credit-analysis)

### Sustainable investment research

The second workflow comes from the **Sustainable Investment Agent for SFDR Article 8 & 9 Funds**. Expand it to follow source inputs through integration, sustainability assessment, stewardship, impact and reporting.

<details>
<summary><b>View the full sustainable-investment workflow</b></summary>

```mermaid
flowchart TD
    subgraph Sources["Primary Sources"]
        S1[Company filings<br/>10-K · 20-F · Annual Report]
        S2[Sustainability reports<br/>CSRD ESRS · TCFD · TNFD]
        S3[Regulatory disclosures<br/>SFDR · UK SDR · Art 29 LEC]
        S4[ESG vendor data<br/>MSCI · Sustainalytics · ISS · S&P]
        S5[NGO and benchmark data<br/>CA100+ · TPI · WBA · CHRB]
        S6[Climate and nature data<br/>PCAF · CBF · SBTi · TPI]
    end

    subgraph PreInv["Pre-Investment Integration"]
        W1[01-04 Materiality · Vendor reconciliation<br/>Exclusions · IC pre-read]
    end

    subgraph SFDR["SFDR Binding Elements"]
        W2[05-07 Art 2-17 SI test · Art 8 monitor<br/>Art 9 stress test]
        W3[08-09 EU Taxonomy alignment · DNSH]
        W4[10-11 PAI issuer dossier · Entity Art 4 statement]
    end

    subgraph Analytics["Thematic & Portfolio Analytics"]
        W5[12-15 TCFD/IFRS S2 · WACI · PCAF · ITR]
        W6[16-18 TNFD LEAP · Biodiversity footprint · EUDR]
        W7[19-21 UNGP salient · HRDD · Living wage/JT]
        W8[22-23 SFDR good governance · EM controlled companies]
    end

    subgraph Active["Active Ownership"]
        W9[24-27 SMART engagement · Log · Collaborative · Escalation]
        W10[28-30 Vote rationale · Say-on-Climate · Shareholder proposals]
        W11[31-32 Controversy 72h memo · Divest vs engage]
    end

    subgraph Impact["Impact & Client"]
        W12[33-36 Theory of Change · IMP 5D · SDG · Avoided emissions]
        W13[37-39 Impact report · Factsheet · Engagement summary]
        W14[40-41 Consultant DDQ · RFP narrative]
    end

    subgraph PortReg["Portfolio & Regulatory"]
        W15[42-44 NGFS Phase V · NZIF 2-0 · S&G KPIs]
        W16[45-46 EM data-gap · Commodity-exporter transition]
        W17[47-49 SFDR Annex IV/V · UK SDR · Art 29 LEC]
        W18[50-52 Energy Paris · Healthcare access · Tech AI governance]
    end

    subgraph Outputs["Institutional Deliverables"]
        O1[IC pre-reads and SI sign-off sheets]
        O2[SFDR periodic disclosure · UK SDR stack<br/>Art 29 LEC report]
        O3[Stewardship Report · Climate Report<br/>Impact Report · Engagement summary]
    end

    S1 --> W1
    S1 --> W2
    S2 --> W5
    S2 --> W6
    S3 --> W4
    S3 --> W17
    S4 --> W1
    S4 --> W2
    S5 --> W7
    S5 --> W9
    S6 --> W5
    S6 --> W15

    W1 --> W2
    W2 --> W3
    W3 --> W4
    W4 --> W5
    W5 --> W8
    W6 --> W8
    W7 --> W8
    W8 --> W9
    W9 --> W10
    W10 --> W11
    W11 --> W12
    W12 --> W13
    W13 --> W14
    W14 --> W15
    W15 --> W16
    W16 --> W17
    W17 --> W18

    W2 --> O1
    W4 --> O2
    W17 --> O2
    W9 --> O3
    W12 --> O3
    W13 --> O3

    %% Profile presentation only; source workflow labels and connections are unchanged.
    classDef default fill:#ecfdf5,stroke:#059669,color:#052e16
    classDef output fill:#065f46,stroke:#065f46,color:#ffffff
    class O1,O2,O3 output
```

[**Explore the source workflow and prompt library →**](https://github.com/HHFinAi/Sustainable-Investment-Agent-for-SFDR-Article-8-9-Funds#workflow-coverage)

</details>

<sub>Reproduced from the projects' workflow documentation on 24 September 2026, with profile-matched colors. Labels and connections are preserved. These copies do not automatically sync with future repository changes; the diagrams are not a certification of regulatory compliance.</sub>
<!-- workflow-charts:end -->

## Selected research projects

<table>
<tr>
<td width="50%" valign="top">
<h3><a href="https://github.com/HHFinAi/Sustainable-Investment-Agent-for-SFDR-Article-8-9-Funds">Sustainable Investment Workflows</a></h3>
<p><b>Bring structure to sustainable investment research.</b></p>
<p>A library of 52 prompts across 18 categories for workflows associated with SFDR Article 8 and 9 strategies, including materiality, climate, stewardship, impact and disclosure research.</p>
<p><code>Sustainable finance</code> <code>Research prompts</code></p>
</td>
<td width="50%" valign="top">
<h3><a href="https://github.com/HHFinAi/Institutional-Growth-Equity-Skills">Institutional Growth Equity Skills</a></h3>
<p><b>From business quality to valuation and deliverables.</b></p>
<p>A bundle of 16 skills spanning competitive positioning, growth research, financial modeling, valuation and research-document production.</p>
<p><code>Growth equities</code> <code>DCF</code> <code>Scenarios</code></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h3><a href="https://github.com/HHFinAi/earnings-analysis">Earnings Analysis</a></h3>
<p><b>Go beyond the headline beat or miss.</b></p>
<p>Parse filings, releases and transcripts; compare results with expectations; diagnose the drivers; and translate changes into the forward research thesis.</p>
<p><code>Filings</code> <code>Guidance</code> <code>Earnings quality</code></p>
</td>
<td width="50%" valign="top">
<h3><a href="https://github.com/HHFinAi/claude-equity-research-skills">Claude Equity Research Skills</a></h3>
<p><b>Make the fundamental research process reusable.</b></p>
<p>Seven composable skills covering growth, competition, earnings, supply chains, corporate networks, investment themes and research reports.</p>
<p><code>Agent skills</code> <code>Fundamental analysis</code></p>
</td>
</tr>
</table>

## Tools and research craft

<p align="center">
  <img src="./assets/toolkit.svg" width="100%" alt="Python for public-data tooling; Markdown for agent instructions; Git for versioned research; GitHub for open collaboration." />
</p>

**Investment research:** `Climate Risk` · `Sustainable Investing` · `Growth Equity` · `Credit Analysis` · `Earnings`

**Research infrastructure:** `Python` · `Agent Skills` · `Structured Evidence` · `Workflow Validation` · `Human Review`

## How I approach the work

**Start with primary sources.** Use company disclosures, filings and documented research inputs—not unsupported narratives.

**Connect the evidence to economics.** Identify the cash-flow, capital-cost, credit or valuation assumption that changes.

**Make uncertainty visible.** Keep scenarios, sensitivities, missing information and disconfirming evidence explicit.

**Keep the analyst accountable.** Automation supports judgment; it does not certify conclusions, guarantee alpha or replace professional review.

## Connect

Working on sustainable finance, public-market research or AI-assisted analysis? Project issues and pull requests are welcome.

<p align="center">
  <a href="https://github.com/HHFinAi/climate-investment-ai-agent-in-equity-and-bond-markets/issues"><b>Start a project discussion</b></a> &nbsp; · &nbsp;
  <a href="https://github.com/hh-health-AI"><b>Explore my sector equity research</b></a>
</p>

---

<p align="center"><sub>Research and educational tools—not investment advice or a certification of regulatory compliance.<br />Prompt libraries require current-source verification; inspect each repository's implementation and limitations.</sub></p>
