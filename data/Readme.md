## Data

### 1. **`evaluation`**
   - Data to evaluate RAG-system
   - Contains Query, Ground Truth, Relevant Text, Domain, URL

### 2. **`evaluation_llm_prompts`**
   - Stores evaluation data that incorporates metrics obtained via LLM-based evaluation.
   - Each entry evaluates the pipeline's outputs against:
     - Query and ground truth answers.
     - Retrieved contexts.
     - Generated responses.
   - **LLM-Based Metrics**:
     - **Relevance**: Measures how well the generated response addresses the query.
     - **Accuracy**: Compares the generated response to the ground truth answer.
     - **Faithfulness**: Assesses how closely the generated response aligns with the retrieved contexts.
   - Additional metrics like **cosine similarity**, **BLEU**, and **ROUGE** scores are also included for deeper quantitative analysis.

### 3. **`experiments`**
   - Contains evaluation results similar to the `evaluation_llm_prompts` folder but excludes LLM-based evaluation metrics.
   - Useful for comparing intrinsic performance without relying on LLMs.

### 4. **`processed`**
   - Preprocessed and cleaned **Cleantech data** used as input for the RAG pipeline.
   - Data has undergone cleaning.
   - Represents the ready-to-use dataset for running experiments and evaluations.

### 5. **`raw`**
   - Raw, unprocessed Cleantech data collected from various sources.
   - Requires cleaning and preprocessing before being used in the RAG pipeline.
   - This serves as the base dataset for generating the data in the `processed` folder.
     
