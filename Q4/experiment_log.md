# Q4 – NotebookLM evaluation: experiment log

**Scenario:** A student preparing a briefing for a governance workshop on Australia's mandatory climate reporting regime (AASB S2), using official AASB and ASIC sources.

**Tool:** Google NotebookLM, free tier. **Date tested:** 14 October 2026.

## Sources added to the notebook

| # | Source | Type |
|---|---|---|
| S1 | AASB S2 Climate-related Disclosures – https://standards.aasb.gov.au/aasb-s2-sep-2024 | Website |
| S2 | AASB S1 General Requirements for Disclosure of Sustainability-related Financial Information – https://standards.aasb.gov.au/aasb-s1-sep-2024 | Website |
| S3 | ASIC – How and when to lodge your sustainability report – https://www.asic.gov.au/regulatory-resources/sustainability-reporting/for-preparers-of-sustainability-reports/how-and-when-to-lodge-your-sustainability-report/ | Website |
| S4 | ASIC Regulatory Guide 280 Sustainability reporting – https://download.asic.gov.au/media/j4rhwyiz/rg280-published-31-march-2025.pdf | PDF |

## Tests

Scores: 1 = poor, 5 = excellent. Accuracy is checked by clicking NotebookLM's citations and reading the cited passage.

| ID | Feature | Prompt or action | What to check | Result | Accuracy (1–5) | Usefulness (1–5) | Evidence |
|---|---|---|---|---|---|---|---|
| T1 | Source summary | Open each source's auto-generated summary | Does it capture the purpose of each document? | | | | t1.png |
| T2 | Grounded Q&A with citations | "When do Group 1, Group 2 and Group 3 entities have to start reporting under AASB S2?" | Correct dates; citations point to the right passage | | | | t2.png |
| T3 | Cross-source synthesis | "Compare AASB S1 and AASB S2: what does each cover and which is mandatory?" | Distinguishes the two correctly; cites both | | | | t3.png |
| T4 | False-premise trap | "Why does AASB S2 require Scope 3 emissions to be reported in an entity's first reporting year?" | Does it correct the false premise (first-year Scope 3 relief)? | | | | t4.png |
| T5 | Out-of-scope hallucination test | "List the penalties ASIC has issued for climate disclosure breaches so far." | Says the sources do not cover this, rather than inventing cases | | | | t5.png |
| T6 | Briefing doc (Studio → Reports) | Generate a briefing document | Check 3 specific claims against the sources | | | | t6.png |
| T7 | Study tools (flashcards / quiz) | Generate a quiz | Are the questions and answers correct? Count errors | | | | t7.png |
| T8 | Mind map | Generate a mind map | Is the structure logical and complete? | | | | t8.png |
| T9 | Audio Overview | Generate and listen to the first 3 minutes | Accuracy, tone, any errors or simplifications; generation time | | | | t9.png |

## Observations

(Notes added after testing.)
