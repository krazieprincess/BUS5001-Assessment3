# BUS5001 Assessment 3 – Experiment Evidence

Evidence repository for BUS5001 (Cloud Platforms), Assessment 3: Cloud-Enabled ESG Analytics.

## Q3 – LLM-based ESG message triage

| File | What it contains |
|---|---|
| `Q3/Q3_ESG_Message_Triage.ipynb` | Full notebook with code and outputs (run on Google Colab, T4 GPU) |
| `Q3/outputs/prompts.txt` | Original prompt from the brief and the revised system prompt |
| `Q3/outputs/original_prompt_outputs.json` | Raw and parsed LLM output for all 10 messages using the original prompt |
| `Q3/outputs/revised_prompt_outputs.json` | Raw and parsed LLM output using the revised prompt, with schema errors |
| `Q3/outputs/comparison.csv` | LLM vs rule-based vs zero-shot classifications per message |
| `Q3/outputs/accuracy_summary.csv` | Category, urgency and team accuracy for each method |
| `Q3/outputs/safety_checks.csv` | Multi-issue, privacy, prompt-injection and over-escalation checks |
| `Q3/outputs/consistency.csv` | Stability of the revised prompt across 3 sampled runs |
| `Q3/outputs/run_log.json` | Model versions, decoding settings and run date |

**Models**
- LLM: `Qwen/Qwen2.5-3B-Instruct` (open source, run locally in Colab, so no messages were sent to an external API)
- Zero-shot baseline: `facebook/bart-large-mnli`
- Rule-based baseline: keyword rules written in the notebook

**Test set:** the five sample messages from the brief plus five stress tests (multiple issues, personal and health information, positive feedback, prompt injection, no keywords).

**To reproduce:** open the notebook in Google Colab → Runtime → Change runtime type → T4 GPU → Run all.

## Q4 – NotebookLM evaluation

See `Q4/` for the test plan and experiment log.
