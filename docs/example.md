---
title: Statement Analysis 
nav_order: 3
---

# Examples
{: .no_toc }

{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

---

### Key Findings on Statement Analysis
- `expr_stmt` has the highest number of samples, followed by `decl_stmt`.  
- `expr_stmt` may augment data via function calls or save data to local variables.  
- Privacy label type has minimal effect on statement distribution.  

### Implications of Statement Analysis
1. **Focus on key statements:**  
  - `expr_stmt` is most associated with privacy behaviors, followed by `decl_stmt` and `if_stmt`.  
  - Statements involving function calls or mathematical operations are likely to implement privacy behaviors.  
  - For `if_stmt`, statements inside the block are more likely to involve privacy behaviors.  

2. **Privacy label has little effect on the order of statement categories**  
  - Order of statement categories is not heavily affected by the privacy label for a single method.  
  - Annotators may need to consider method call graphs or dependencies for accurate labeling.  
  - Knowing data is read by a third-party API is insufficient without considering dependent method calls.

### Statement Distribution Table

This table shows a normalized distribution of participant ratings across statement categories for the four "purpose" privacy behaviors (excluding `func_call`):

| Statement        | Ad    | Func  | Analyt | Other |
|-----------------|-------|-------|--------|-------|
| `expr_stmt`      | 48.7  | 49.9  | 58.5   | 48.4  |
| `if_stmt`        | 21.8  | 20.1  | 16.1   | 20.7  |
| `decl_stmt`      | 21.8  | 21.5  | 17.8   | 21.2  |
| `return`         | 4.2   | 5.1   | 3.5    | 6.2   |
| `function_sig`   | 1.1   | 0.9   | 2.6    | 0.9   |
| `case`           | 0.3   | 0.3   | 0.3    | --    |
| `argument`       | --    | 0.9   | --     | --    |
| `try`            | --    | --    | --     | 0.5   |
