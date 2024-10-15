# Pre-experiment Checks

This folder contains preliminary tests and experiments to verify the functionality of various components (e.g., prompting stratagies, parsing) before starting major experiments. Below is a record of the tests conducted, including their purpose, date, and related files.

---

## Experiment Log

- **Date**: 2024-10-15
- **Purpose**:  To verify that the `parse_fol.py` script correctly generates and parses a CFG for FOL expressions.
- **Files**: 
  - `test_Parse_FOL.ipynb`: Colab notebook for test the lexer, dynamic cfg generator, parser function 
  - `parse_fol.py`:  Python script that generates the CFG for FOL expressions and performs the parsing.
- **Results**:
  - The script successfully generated CFGs and parsed simple FOL expressions  
- **Next Steps**:
  - test robustness of parser by using more complex and varied test cases.
  - evaluating similarity between different parse trees and testing the performance of LE similarity metrics.
