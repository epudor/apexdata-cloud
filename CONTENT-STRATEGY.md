# Apex Data Cloud — Content Strategy & Backlog

This is the editorial backlog that feeds the architecture already built. Items marked **✅ built** ship in this repo today; everything else is prioritized below. Excluded from the Jekyll build.

Priority key: **P1** = build first (high traffic × high intent × easy), **P2** = next, **P3** = long-tail / fill-in.

---

## 100 Article Topics (for `/resources/blog/`, in `_posts/`)

### Cluster A — AI Strategy & Adoption (supports /services/ai-consulting/)
1. Why AI projects fail — and how to avoid it ✅ built
2. How to build an AI roadmap in 30 days — **P1**
3. AI use-case prioritization: a scoring framework — **P1**
4. Build vs. buy: when to develop AI in-house — **P1**
5. How much does an AI project cost? — **P1**
6. The AI readiness checklist for mid-market companies — **P1**
7. AI governance for companies that aren't Google — **P2**
8. How to measure AI ROI — **P1**
9. The hidden costs of "free" AI pilots — **P3**
10. AI strategy for non-technical executives — **P2**
11. When NOT to use AI — **P2**
12. From POC to production: the AI deployment gap — **P1**
13. Responsible AI: a practical playbook — **P2**
14. AI vendor selection: questions to ask — **P3**
15. Change management for AI adoption — **P3**

### Cluster B — Generative AI, RAG & Agents (supports /services/generative-ai-consulting/, /rag-development/, /ai-agent-development/)
16. RAG vs. fine-tuning: when to use each ✅ built
17. How to build a production RAG system — **P1**
18. Why your RAG system gives wrong answers (and fixes) — **P1**
19. Chunking strategies for RAG, compared — **P2**
20. How to evaluate a RAG system — **P1**
21. Choosing a vector database — **P2**
22. GPT vs. Claude vs. Gemini for enterprise — **P1**
23. What are AI agents, really? — **P1**
24. Single-agent vs. multi-agent architectures — **P2**
25. How to keep LLM costs under control — **P1**
26. Preventing hallucinations in production LLMs — **P1**
27. Prompt engineering that actually scales — **P2**
28. Should you self-host an open-source LLM? — **P2**
29. Building an internal knowledge assistant — **P1**
30. AI copilots for customer support — **P2**
31. Guardrails for enterprise GenAI — **P2**
32. Fine-tuning: when it's worth it — **P2**
33. RAG for regulated industries — **P3**
34. Evaluating LLM outputs at scale — **P3**
35. The economics of generative AI at scale — **P3**

### Cluster C — Machine Learning (supports /services/machine-learning-consulting/)
36. Customer churn prediction: a practical guide — **P1**
37. Demand forecasting with machine learning — **P1**
38. Lead scoring models that work — **P1**
39. What is MLOps and why you need it — **P1**
40. How to detect and fix model drift — **P2**
41. Feature stores explained — **P2**
42. Recommendation engines for any catalog size — **P2**
43. Propensity modeling 101 — **P2**
44. Model explainability for regulated decisions — **P2**
45. How much data do you need for ML? — **P1**
46. Building vs. buying a forecasting solution — **P3**
47. A/B testing for ML models — **P3**
48. Time-series forecasting methods compared — **P3**
49. Reducing false positives in fraud models — **P3**
50. From dashboard to decision: operationalizing ML — **P2**

### Cluster D — Data Engineering, Cloud & Governance (supports /data-engineering/, /cloud-architecture/, /data-governance/)
51. Data warehouse vs. lakehouse — **P1**
52. The modern data stack, explained — **P1**
53. How to cut cloud data costs — **P1**
54. dbt: what it is and why it matters — **P2**
55. Batch vs. streaming data pipelines — **P2**
56. Building a customer data platform (CDP) — **P2**
57. Data quality: a practical framework — **P1**
58. Data governance without bureaucracy — **P2**
59. GDPR & CCPA for data teams — **P2**
60. Master data management explained — **P3**
61. Snowflake vs. Databricks vs. BigQuery — **P1**
62. Data observability: catching issues early — **P2**
63. Reverse ETL and data activation — **P3**
64. How to migrate to a lakehouse — **P3**
65. Data contracts explained — **P3**
66. Real-time analytics architectures — **P3**
67. Cloud security for data platforms — **P2**
68. FinOps for data teams — **P2**
69. Choosing a cloud provider for AI workloads — **P2**
70. Designing for data scalability — **P3**

### Cluster E — Analytics, Segmentation & Growth (supports /customer-segmentation/, /marketing-analytics/)
71. Customer segmentation that drives revenue ✅ built
72. Marketing attribution after third-party cookies — **P1**
73. Multi-touch attribution vs. marketing mix modeling — **P1**
74. RFM segmentation: a step-by-step guide — **P1**
75. Measuring true marketing incrementality — **P2**
76. CAC and LTV: getting the math right — **P1**
77. Building a marketing data warehouse — **P2**
78. Predictive segmentation with ML — **P2**
79. Personalization that lifts conversion — **P2**
80. Marketing dashboards executives actually use — **P2**
81. Lookalike audiences from first-party data — **P3**
82. Churn analytics for subscription businesses — **P2**
83. Pipeline forecasting for B2B — **P3**
84. Attribution for long sales cycles — **P3**
85. The death of the cookie: what to do now — **P2**

### Cluster F — Industry & Local (supports /industries/*, /locations/*)
86. AI use cases in healthcare — **P1**
87. AI in financial services: top use cases — **P1**
88. AI for retail and e-commerce — **P1**
89. AI in manufacturing: where to start — **P2**
90. AI for SaaS growth — **P2**
91. AI in real estate — **P2**
92. AI consulting in Orlando: a local guide — **P2**
93. Florida's AI economy: opportunities — **P3**
94. Predictive maintenance for manufacturers — **P3**
95. HIPAA-conscious AI in healthcare — **P3**

### Cluster G — Thought Leadership / GEO bait
96. The state of enterprise AI (annual) — **P2**
97. 2026 AI trends for business leaders — **P2**
98. AI buzzwords decoded for executives — **P3**
99. What we learned shipping AI to production — **P3**
100. The Apex approach to AI engagements — **P3**

---

## 50 FAQ Topics
*(Deploy as `faqs:` front-matter blocks on the most relevant page — each emits FAQPage schema automatically. Build P1s into existing pages first.)*

1. What does an AI consultant do? ✅ (ai-consulting)
2. How much does AI consulting cost? — **P1** (ai-consulting)
3. How long does an AI project take? ✅ (homepage/ai-consulting)
4. What's the difference between AI and machine learning? — **P1** (glossary/ai-consulting)
5. What is generative AI? ✅ (glossary)
6. What is RAG? ✅ (glossary)
7. RAG vs. fine-tuning — which is better? ✅ (comparison)
8. What is an AI agent? ✅ (glossary)
9. Do we need clean data before starting AI? ✅ (ai-consulting)
10. How do you measure AI ROI? — **P1**
11. Is our data ready for AI? — **P1** (ai-readiness)
12. GPT vs. Claude vs. Gemini — which to use? — **P1**
13. What is MLOps? ✅ (glossary)
14. What is a vector database? ✅ (glossary)
15. What are embeddings? ✅ (glossary)
16. What is a data lakehouse? ✅ (glossary)
17. Warehouse or lakehouse — which do we need? ✅ (data-engineering/comparison)
18. Snowflake vs. Databricks? ✅ (comparison)
19. How do you prevent AI hallucinations? ✅ (generative-ai)
20. Is our data GDPR/CCPA compliant? — **P1** (data-governance)
21. What is data governance? ✅ (data-governance)
22. What is customer segmentation? ✅ (customer-segmentation)
23. RFM vs. predictive segmentation? ✅ (customer-segmentation)
24. What is marketing attribution? ✅ (marketing-analytics)
25. Attribution vs. marketing mix modeling? ✅ (marketing-analytics)
26. Will analytics work without cookies? ✅ (marketing-analytics)
27. What is churn prediction? — **P2**
28. What is demand forecasting? — **P2**
29. What is lead scoring? ✅ (real-estate)
30. How do you control LLM costs? — **P1**
31. Should we self-host an LLM? — **P2**
32. What is fine-tuning? ✅ (glossary)
33. Build vs. buy AI? — **P1**
34. How do you choose AI use cases? ✅ (ai-consulting)
35. What industries do you serve? ✅ (homepage)
36. Where are you located? ✅ (homepage/locations)
37. Do you work remotely / nationwide? ✅ (locations)
38. How is this different from an agency? ✅ (homepage)
39. What is predictive vs. generative AI? ✅ (comparison)
40. How much data do we need for ML? — **P2**
41. What is model drift? — **P2** (glossary candidate)
42. What is a CDP? — **P2** (glossary candidate)
43. How do you ensure data quality? ✅ (data-engineering)
44. What is MMM? ✅ (marketing-analytics)
45. Can AI improve retention? ✅ (financial-services)
46. What is predictive maintenance? ✅ (manufacturing)
47. How do you handle HIPAA / patient data? ✅ (healthcare)
48. What is product-led growth analytics? ✅ (technology)
49. How do we get started? ✅ (orlando/contact)
50. Is the assessment really free? ✅ (ai-readiness)

---

## 25 Case Study Ideas (collection: `_case_studies/`)
*(Anonymize until named clients approve. Two ✅ built as representative examples.)*

1. SaaS churn prediction ✅ built
2. RAG knowledge assistant ✅ built
3. Healthcare patient no-show prediction — **P1**
4. Financial services fraud detection — **P1**
5. Retail recommendation engine — **P1**
6. Manufacturing demand forecasting — **P1**
7. Marketing attribution rebuild (post-cookie) — **P1**
8. Cloud cost reduction (data platform) — **P1**
9. Lead scoring for B2B sales — **P2**
10. Customer segmentation → campaign lift — **P2**
11. Support copilot deployment — **P2**
12. Data lakehouse migration — **P2**
13. CDP implementation — **P2**
14. Predictive maintenance pilot — **P2**
15. Generative AI content system — **P2**
16. AI agent for ops automation — **P2**
17. Data governance / GDPR program — **P3**
18. Real estate lead intent model — **P3**
19. Subscription churn + retention offers — **P3**
20. Demand forecasting for inventory — **P3**
21. Executive marketing dashboard — **P3**
22. MLOps platform stand-up — **P3**
23. LLM cost optimization — **P3**
24. Data quality turnaround — **P3**
25. AI readiness → roadmap engagement — **P3**

---

## 25 Comparison Pages (collection: `_comparisons/`)
1. RAG vs. fine-tuning ✅ built
2. Data warehouse vs. lakehouse ✅ built
3. Generative AI vs. predictive AI ✅ built
4. GPT vs. Claude vs. Gemini — **P1**
5. Snowflake vs. Databricks — **P1**
6. Snowflake vs. BigQuery — **P2**
7. Build vs. buy AI — **P1**
8. In-house vs. AI consulting firm — **P1**
9. Multi-touch attribution vs. MMM — **P1**
10. Pinecone vs. Weaviate vs. pgvector — **P2**
11. Batch vs. streaming pipelines — **P2**
12. ETL vs. ELT — **P2**
13. Data lake vs. data warehouse — **P2**
14. AI agent vs. chatbot — **P2**
15. Open-source vs. proprietary LLMs — **P2**
16. Single-agent vs. multi-agent — **P3**
17. Supervised vs. unsupervised learning — **P3**
18. dbt vs. stored procedures — **P3**
19. AWS vs. Azure vs. GCP for data/AI — **P1**
20. Fivetran vs. custom ingestion — **P3**
21. CDP vs. data warehouse — **P2**
22. First-party vs. third-party data — **P2**
23. Marketing agency vs. analytics consultancy — **P2**
24. Rule-based vs. ML segmentation — **P3**
25. Prompt engineering vs. fine-tuning — **P3**

---

## 25 Glossary Pages (collection: `_glossary/`)
1. Retrieval-augmented generation (RAG) ✅ built
2. MLOps ✅ built
3. Embeddings ✅ built
4. Vector database ✅ built
5. Large language model (LLM) ✅ built
6. Fine-tuning ✅ built
7. AI agent ✅ built
8. Generative AI ✅ built
9. Data lakehouse ✅ built
10. Predictive analytics — **P1**
11. Machine learning — **P1**
12. Customer data platform (CDP) — **P1**
13. Model drift — **P2**
14. Feature store — **P2**
15. Data pipeline (ETL/ELT) — **P1**
16. Marketing attribution — **P1**
17. Customer lifetime value (LTV) — **P1**
18. Churn rate — **P2**
19. Prompt engineering — **P2**
20. Hallucination (AI) — **P2**
21. Data governance — **P1**
22. Data warehouse — **P1**
23. Natural language processing (NLP) — **P2**
24. Supervised learning — **P3**
25. Semantic search — **P2**

---

## Internal linking rules
- Every **service** links to ≥3 related services + its industry/assessment.
- Every **glossary** term links to ≥1 service + ≥1 related term/comparison.
- Every **comparison** links to the relevant service + glossary terms.
- Every **article** links up to its pillar (service) and sideways to 2 related articles.
- Every page links to **/contact/** and a relevant **/assessments/** page (handled by the `page` layout sidebar + CTA band).
