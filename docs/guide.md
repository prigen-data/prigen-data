---
title: Dataset Guide 
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

### Data Structure

The dataset is organized as a **dictionary**, where each key is a **unique function ID** and the value is another dictionary containing:

- `code`: Full function code.
- `label`: Privacy behavior in the purpose label.
- `first`, `second`, `third`: Up to three annotated statements representing the most important statements for privacy. If no statement is annotated, the field is `NULL`.


### Data format

| Field        | Example Value                 | Explanation |
|--------------|-------------------------------|-------------|
| `function_id`| `function_id_001`             | Unique identifier for this function in the dataset, used as the dictionary key. |
| `code`       | `public static com.heyzap.common.net.Connectivity$OpenRtbConnectionType openRtbConnectionType(android.content.Context p3){...}` | Full function code. |
| `label`      | `purpose-Advertisement`               | Privacy purpose label. |
| `first`      | `public static com.heyzap.common.net.Connectivity$OpenRtbConnectionType openRtbConnectionType(android.content.Context p3)`                        | First-level important statement. `NULL` means there is no relevant statement. |
| `second`     | `com.heyzap.common.net.Connectivity$OpenRtbConnectionType v0_1 = v0_5.getSubtype();`                        | Second-level important statement. `NULL` means there is no relevant statement. |
| `third`      | `com.heyzap.common.net.Connectivity$OpenRtbConnectionType v0_5 = ((android.net.ConnectivityManager) p3.getSystemService(connectivity)).getActiveNetworkInfo();`                        | Third-level important statement. `NULL` means there is no relevant statement. |




### Statistics of Dataset

| Description                             | Numbers |
|-----------------------------------------|--------|
| Total number of annotated functions     | 2,426  |
| Total number of functions with single annotation | 2,167 |
| Total number of functions with duplicate annotations | 259 |
| Total number of privacy behaviors       | 4      |
| Total number of relevant statements per function | 3 |
| Total number of unique participants     | 18     |
| Mean number of lines of function        | 26     |
| Mean cyclomatic complexity of functions | 5      |
| Maximum cyclomatic complexity of functions | 86   |
| Minimum cyclomatic complexity of functions | 1    |
