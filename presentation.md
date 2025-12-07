---
marp: true
theme: gaia
paginate: true
author: Technical Writer
backgroundColor: #fff
style: |
  section {
    font-family: 'Arial', sans-serif;
    font-size: 28px;
  }
  h1 {
    color: #2c3e50;
  }
  /* Custom class for code slides */
  section.code-slide {
    background-color: #f4f4f4;
  }
---

<!-- _class: lead -->

# Product Documentation: API V2
## Technical Specification & Deployment

**Contact:** 23f3000339@ds.study.iitm.ac.in

---

<!-- _header: **Overview** -->
<!-- _footer: Q4 Roadmap -->

## Presentation Scope

This documentation covers the transition to our new search architecture.

- **Versioning**: Semantic Versioning 2.0.0
- **Format**: RESTful JSON
- **Status**: <span style="color:green">Production Ready</span>

---

<!-- Background image slide -->
![bg brightness:0.4](https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&w=1920&q=80)

# Infrastructure
## Cloud-Native Deployment

Our microservices are orchestrated using Kubernetes, allowing for zero-downtime updates and auto-scaling.

---

## Algorithmic Efficiency

To maintain sub-millisecond response times, we optimized the indexing algorithm. 

The time complexity for our new inverted index search is:

$$
T(n) = O(k \cdot \log n)
$$

Where:
- $n$ is the total number of documents
- $k$ is the number of query terms

---

<!-- _class: code-slide -->

## Implementation Example

The core indexer is implemented in Python:

```python
def calculate_complexity(n, k):
    """
    Calculate theoretical max operations
    """
    import math
    if n <= 0: return 0
    return k * math.log(n, 2)


<!-- _backgroundColor: #2c3e50 -->
<!-- _color: white -->
Thank You
For documentation access, please contact:
23f3000339@ds.study.iitm.ac.in


Code
***

### Answer to "What is the raw GitHub URL?"

To access the raw content of a file stored in a GitHub repository (which is required if you want to load a Marp presentation directly from a URL or pipe it into a CI/CD build), the URL format is:

**`https://raw.githubusercontent.com/[USER]/[REPO]/[BRANCH]/[PATH_TO_FILE]`**

**Example:**
If your username is `johndoe`, the repo is `docs`, the branch is `main`, and the file is `slides.md`:

`https://raw.githubusercontent.com/johndoe/docs/main/slides.md`
