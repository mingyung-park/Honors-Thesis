# Pre-experiment Checks

This folder contains preliminary tests and experiments to verify the functionality of various components (e.g., prompting stratagies, parsing) before starting major experiments. Below is a record of the tests conducted, including their purpose, date, and related files.

---

## Experiment Log

#### 4. Pairwise Similarity Calculation
**Date**: 2024-10-28 
```
- **Purpose**:
  To validate the functionality of the pairwise similarity calculation module. This experiment aims to ensure that pairwise LE, BLEU, and weighted scores between multiple FOL expressions are calculated accurately and consistently.

- **Files**:
  - `test_Pairwise_Similarity.ipynb`: Jupyter notebook containing tests for pairwise similarity metrics, including LE score evaluation, BLEU score calculation, and weighted score computations.

- **Results**: The notebook successfully computed pairwise similarity scores for various FOL expression pairs. Results were consistent with expected behavior for both LE and BLEU metrics.
- **Next Steps**: Integrate the tested module into the main pipeline for consistency evaluation.
```
#### 3. LE Module
**Date**: 2024-10-28 
```
- **Purpose**: To test the LE (Logical Equivalence) module's ability to correctly evaluate logical equivalence between FOL expressions using truth table generation and comparison. This test ensures the LE module accurately identifies logically equivalent and non-equivalent FOL pairs.
- **Files**:  `test_LE_module.ipynb`: Jupyter notebook for testing the LE module. It includes procedures for FOL expression parsing, truth table generation, and comparison logic.
- **Results**:  
  - The module successfully identified equivalence for several pairs of FOL expressions. It also handled cases where expressions differed in structure but were logically equivalent.
- **Next Steps**:  
  - Test the module in combination with other metrics, such as BLEU and weighted scoring, within the overall pipeline.
```
  
#### 2. LE Score Calculation
**Date**: 2024-10-24  
```
- **Purpose**:  To validate that the LE (Logical Equivalence) Score Calculation script accurately evaluates the similarity between FOL (First-Order Logic) expressions. This test ensures that the LE score calculation provides consistent results when comparing two FOL expressions.
- **Files**:
  - `test_LE_calculation.ipynb`: Colab notebook for testing the LE score calculation, including FOL expression parsing, truth table generation, and evaluation of similarity metrics.
- **Results**: The script successfully generated truth tables for both expressions and matched the literals correctly.
- **Next Steps**: Further tests are required to handle edge cases with unequal literal counts and expressions with nested quantifiers. Integration with the main experiment pipeline to measure LE score in combination with other metrics.
```
#### 1. Parsing FOL Expressions

**Date**: 2024-10-15
```
- **Purpose**:  To verify that the `parse_fol.py` script correctly generates and parses a CFG for FOL expressions.
- **Files**: 
  - `test_Parse_FOL.ipynb`: Colab notebook for test the lexer, dynamic cfg generator, parser function 
- **Results**:
  - The script successfully generated CFGs and parsed simple FOL expressions  
- **Next Steps**:
  - test robustness of parser by using more complex and varied test cases.
  - evaluating similarity between different parse trees and testing the performance of LE similarity metrics.
```
