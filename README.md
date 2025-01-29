# Financial Discrepancy Categorization
Automated financial discrepancy categorization
*   **Problem:** This project addresses the challenge of automating financial discrepancy categorization and resolution.
*   **Approach:** The approach involves preprocessing financial data, categorizing discrepancies using keywords and potentially LLM semantic understanding, and automating actions based on resolution status. BART (`facebook/bart-large-cnn`) is employed as the LLM for text generation tasks (summarization, next steps, and pattern identification).  Batch processing with Hugging Face Datasets is used to efficiently process large datasets and leverage GPU acceleration.
*   **Model Explanation:** BART is chosen for its strong performance in text generation and summarization tasks. The `facebook/bart-large-cnn` model is used for its balance between performance and resource requirements.  Preprocessing steps include handling missing values, converting data types, and normalizing text for consistent keyword matching.  The `datasets` library is used for efficient batch processing with BART.
*   **Evaluation:** The solution is evaluated based on accuracy (how well it categorizes discrepancies), performance (processing speed), code quality, scalability, and explainability (clarity of LLM prompts and outputs).  A portion of the input data should be reserved as a test set and kept separate from the development process.
