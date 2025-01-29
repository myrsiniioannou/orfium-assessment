# Text Normalization Assessment Report

## Objective
The goal was to design a system to normalize raw composer/writer data by removing redundant or irrelevant information while retaining valid names.

## Approach
1. **Text Preprocessing**:
   - Unified delimiters (`/`, `,`, `&`) and cleaned segments using regex.
   - Removed irrelevant patterns like placeholders, numeric data, and publisher names.
2. **Entity Recognition**:
   - Used spaCy’s multilingual model to identify PERSON entities for normalization.
3. **Name Reordering**:
   - Reordered names in "Lastname, Firstname" format for consistency.
4. **Normalization**:
   - Combined cleaned and validated names into a single normalized output.

## Evaluation
- **Exact Match**: Achieved a match rate of X%.
- **Jaccard Similarity**: Average similarity score of Y%.
- **Visualization**:
   - Distribution of Jaccard Similarities showed Z% of rows with high overlap.

## Recommendations
1. **Fine-Tune spaCy Models**:
   - Train domain-specific NER models for better recognition.
2. **Introduce Supervised Learning**:
   - Develop a machine learning model for improved accuracy.
3. **Enhance Unicode Handling**:
   - Improve processing of non-Latin characters.
