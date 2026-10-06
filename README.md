<p align="center">
  <a href="https://alex-labou.vercel.app/en">
    <img src="./assets/profile-banner.svg" width="100%" alt="Komla Alex Labou — Data & AI Engineer" />
  </a>
</p>

<p align="center">
  <a href="https://alex-labou.vercel.app/en"><img src="https://img.shields.io/badge/Portfolio-alex--labou.vercel.app-93A4FF?style=for-the-badge&logo=vercel&logoColor=white&labelColor=0B0D13" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/komla-alex-labou/"><img src="https://img.shields.io/badge/LinkedIn-Komla%20Alex%20Labou-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0B0D13" alt="LinkedIn" /></a>
  <a href="mailto:alexlabou03@gmail.com"><img src="https://img.shields.io/badge/Email-alexlabou03%40gmail.com-34D399?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0B0D13" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Open%20to-AI%20%26%20ML%20roles-A77BFF?style=for-the-badge&labelColor=0B0D13" alt="Open to AI and ML roles" />
</p>

<p align="center">
  <strong>Data & AI Engineer · ENSAI Rennes & ENSAE Dakar · based in France</strong><br/>
  I build data platforms, models and agents whose evidence can be checked, performance measured and limitations understood.
</p>

---

## Now · CEPS Data Platform & Explorer

<a href="https://alex-labou.vercel.app/en/projects/ceps">
  <img src="./assets/ceps-card.svg" width="100%" alt="CEPS Data Platform & CEPS Explorer: 15 sources, ~41M rows, 105 SQL views, 267 tests" />
</a>

At the **CEPS** (Economic Committee for Health Products, Paris), I am the **sole designer and developer** of the data platform and business application used to prepare medicine-price negotiations.

- **The problem:** sales, reimbursement, hospital, rebate and regulatory data scattered across files with competing identifiers.
- **What I built:** source adapters, identifier normalization, history preservation, 113 versioned SQL migrations, a read-only FastAPI service and a Next.js application for business teams — growth decomposition by price, volume and mix, HAS pathways, exports and product PDFs.
- **Traceability by design:** 442 files tracked by SHA-256, 675 logged ingestion runs, 3,922 recorded data-quality issues, human-approved corrections. No invented identifier mapping; missing stays missing.
- **Next:** user acceptance testing and migration to the ministry's infrastructure (PostgreSQL, Docker).

<sub>Code and data are internal to CEPS · figures as of 30 September 2026 · <a href="https://alex-labou.vercel.app/en/projects/ceps">full case study →</a></sub>

---

## Selected projects

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://alex-labou.vercel.app/en/projects/retailops-ai"><img src="./assets/retailops-card.svg" width="100%" alt="RetailOps AI" /></a>
      <p>Recursive 28-day forecasts turned into explicit inventory scenarios, TreeSHAP explanations and a LangGraph copilot with bounded tools. Leakage-safe dbt layers on BigQuery, training validated on Cloud Run Jobs.</p>
      <sub>Private repository · <a href="https://alex-labou.vercel.app/en/projects/retailops-ai">case study</a> · walkthrough on request</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/EL-K-Code/Job-Copilot"><img src="./assets/jobcopilot-card.svg" width="100%" alt="JobCopilot" /></a>
      <p>Turns a verified candidate profile and a job offer into a reviewable application pack — without inventing skills. Evidence ledger, deterministic claim composition, tenant-isolated memory, supervised Gmail drafts.</p>
      <sub><a href="https://github.com/EL-K-Code/Job-Copilot">Source</a> · <a href="https://alex-labou.vercel.app/en/projects/jobcopilot">case study</a></sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://alex-labou.vercel.app/en/projects/relationscope-nlp"><img src="./assets/relationscope-card.svg" width="100%" alt="RelationScope NLP" /></a>
      <p>Relation classification that calibrates its confidence and abstains on unknown relations: 84.45% unknown rejection, 16 unseen relations held out for the final test. FastAPI/Next.js serving on GCP with Terraform.</p>
      <sub>Private repository · <a href="https://alex-labou.vercel.app/en/projects/relationscope-nlp">case study</a> · with Maxime Ferret (ENSAI)</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/EL-K-Code/evisuff-finance"><img src="./assets/evisuff-card.svg" width="100%" alt="EviSuff Finance" /></a>
      <p>A counterfactual protocol testing whether long-document agents change their answer when answer-critical evidence is removed. Paired bootstrap intervals, abstention and citation metrics, CI-checked benchmark integrity.</p>
      <sub><a href="https://github.com/EL-K-Code/evisuff-finance">Source</a> · research protocol, no empirical model claims yet</sub>
    </td>
  </tr>
</table>

<details>
  <summary><strong>More engineering work</strong></summary>
  <br/>

- **[IMDB Data Platform](https://github.com/EL-K-Code/imdb-data-platform)** — TSV → Parquet → GCS → BigQuery ingestion with chunked processing and a reproducible bronze layer.
- **[KandiaAI](https://github.com/EL-K-Code/kandiai)** — human-centered career intelligence for African professionals, preserving truthful profile representation.
- **[ML Model Serving & Deployment](https://github.com/EL-K-Code/gender-prediction-api)** — FastAPI, Docker, PostgreSQL, Cloud Run and GitHub Actions.
- **[Agentic AI](https://github.com/EL-K-Code/Agentic-AI)** — agent orchestration, tools and structured workflows.
- **[RAG Playground](https://github.com/EL-K-Code/rag-playground)** — compact retrieval-augmented generation experiments.

</details>

---

## Proof, not promises

| Project | Result | Protocol |
| --- | --- | --- |
| **RetailOps AI** | **0.771** mean RMSSE vs 0.952 (best naive baseline) | Same 28-day validation window, 2.7M training rows — not the official M5 WRMSSE |
| **JobCopilot** | **121/121** claims supported · **22/22** in a 10-offer end-to-end audit | Frozen 50-case grounding benchmark, zero detected technology contamination |
| **RelationScope** | **89.16%** Macro-F1 · **84.45%** unknown rejection | Open-set protocol: 56 known relations, 16 unseen held out from calibration |
| **WFP biometrics** | **EER 4.34%** · **AUC 0.981** · **Rank-1 94.5%** | SOCOFing fingerprints, threshold and robustness analysis |

Every metric comes with its protocol, and every project states its limits.

---

## Experience

<table>
  <tr>
    <td width="50%" valign="top">
      <sub>JUNE 2026 — PRESENT · PARIS</sub>
      <h4>Data Science & Data Engineering · CEPS</h4>
      Sole developer of the CEPS Data Platform and CEPS Explorer: 15 sources, history, quality controls, economic analysis, FastAPI and Next.js.
    </td>
    <td width="50%" valign="top">
      <sub>JULY — DEC. 2025 · ROME</sub>
      <h4>Data Scientist · World Food Programme (UN)</h4>
      Fingerprint duplicate-detection prototype for beneficiary identification: MinutiaeNet minutiae extraction and Bozorth3-inspired matching.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <sub>2024 — 2026</sub>
      <h4>ENSAI Rennes · Data Science & Data Engineering</h4>
      Machine learning, deep learning, NLP, cloud and data engineering. Team research on SLA-aware serverless placement across cloud, fog and edge (auction, greedy and RL strategies).
    </td>
    <td width="50%" valign="top">
      <sub>2020 — 2024</sub>
      <h4>ENSAE Dakar · Engineering degree in Statistics & Economics</h4>
      Statistics, econometrics, inference and survey analysis. Research assistant and data analyst roles in Dakar.
    </td>
  </tr>
</table>

---

## Toolkit

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,fastapi,nextjs,ts,postgres,docker,gcp,aws,terraform,githubactions&theme=dark" alt="Core stack" />
</p>

<table>
  <tr>
    <td width="50%" valign="top"><strong>AI / ML / NLP</strong><br/>PyTorch · TensorFlow · scikit-learn · Hugging Face · LightGBM · SHAP · Sentence Transformers</td>
    <td width="50%" valign="top"><strong>LLM systems</strong><br/>LangGraph · RAG · tool calling · structured outputs · FAISS · Pydantic · evidence grounding</td>
  </tr>
  <tr>
    <td width="50%" valign="top"><strong>Data</strong><br/>SQL · DuckDB · BigQuery · dbt · PostgreSQL · data quality & lineage</td>
    <td width="50%" valign="top"><strong>Delivery</strong><br/>FastAPI · Next.js · Docker · GCP · AWS · Terraform · GitHub Actions · GitLab CI</td>
  </tr>
</table>

---

<p align="center">
  <strong>Building data platforms, reliable agents or evaluation-driven ML?</strong><br/>
  <a href="https://alex-labou.vercel.app/en">Portfolio</a> · <a href="https://www.linkedin.com/in/komla-alex-labou/">LinkedIn</a> · <a href="mailto:alexlabou03@gmail.com">alexlabou03@gmail.com</a>
</p>
