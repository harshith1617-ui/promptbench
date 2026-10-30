# PromptBench: Systematic Prompt Evaluation & Optimization Framework


### 1. Problem Formulation
Empirical framework evaluating 6 prompt engineering strategies across 5 task domains (Reasoning, Summarisation, Classification, Structured Extraction, Creative Writing) and 3 LLMs (Llama-3.1-8B, Mistral-7B, Qwen-2.5-7B).

### 2. Evaluated Strategies
1. Zero-Shot (Baseline)
2. Few-Shot (3 Solved Exemplars)
3. Chain-of-Thought (Step-by-Step Reasoning)
4. Self-Consistency (5-Path Majority Voting)
5. Role Prompting (Domain Expert Persona)
6. Structured-Output (Strict JSON Schema)

### 3. Datasets
- GSM8K (Math Reasoning)
- CNN / DailyMail (Summarisation)
- Stanford SST-2 (Classification)
- CoNLL-2003 (Structured Extraction)
- WritingPrompts (Constrained Creative Writing)

### 4. Key Findings
- **Reasoning:** Self-Consistency achieves 84.6% (+22.4% over baseline); Chain-of-Thought is Pareto-optimal (+16.2% under 1s).
- **Classification:** Few-Shot reaches 91.4% in 390 ms; Self-Consistency uses 5.5x compute for only +0.3% gain.
- **Data Pipelines:** Structured-Output raises valid JSON parsing from 71.4% to 98.2%.
- **Creative:** Role Prompting wins on human preference (4.56 / 5.0).

### 5. Deployment on GitHub Pages
1. Go to repository **Settings** -> **Pages**.
2. Source: **Deploy from a branch**.
3. Branch:  /  -> Click **Save**.
