# bible-chatgpt-prompts
---
license: cc0-1.0
tags:
- ChatGPT
- Bible
- Theology
- Christian Apologetics
task_categories:
- text-generation
- question-answering
size_categories:
- 1K<n<10K
---

<p align="center">
  <h1 align="center">🧠📖 Bible ChatGPT Prompts [CSV Dataset]</h1>
</p>

A curated collection of specialized ChatGPT prompts for biblical studies, theological research, and Christian apologetics. This dataset enables AI assistants to provide nuanced analysis of scripture, theological concepts, and historical religious contexts. Additional prompts included for all religions, philosophies, sciences, and other areas of study, e.g., anthropology, mathematics, and computer science.

## Features

- 5 detailed prompt templates for theological AI interactions
- Focused on key areas: Dispensationalism, Eschatology, Ecclesiology, Soteriology
- CSV format for easy integration with AI applications
- Includes prompts for comparative religious studies

## Dataset Structure
```
Act,Prompt
"Bible Scholar 1","I need help categorizing aspects of Dispensationalism..."
```


## Contributing
Contributions welcome! Please:
1. Open an issue to discuss proposed changes
2. Fork the repository
3. Submit a pull request with updated prompts

## License
[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) - No rights reserved. Attribution appreciated but not required.


## LLM Code Generation Notice

Portions of this codebase were generated or refined using large language models (LLMs) including models such as Gemini, ChatGPT, Claude, DeepSeek, Qwen, Dolphin-Llama, and more, integrated API Plugins Such as Cline, Continue, Roo Code, and more, and Service Providers such as OpenRouter, Ollama, HuggingFace, Cursor, and GitHub Copilot and more. Final code was reviewed and adapted by the project maintainer. Use at your own risk.

# Limitation of Liability Statement and Statement of Copyright Protection

For a complete Limitation of Liability Statement, please visit [link](https://docs.google.com/document/d/1F8WUkStTyV0ZcsjluN9WtvUm29hRzqNtZ7GcNX76acA/edit?usp=sharing) and [link](https://docs.google.com/document/d/1q4zYgmg0Aoo5_5znIlJDfmD7coEDaDh5KLCaxHiKQOI/edit?usp=sharing).


# Orthogonal Prompt Engineering: High-Dimensional Creative Methodology

This README provides a structured introduction to the methodology of prompt engineering using high-dimensional orthogonal vector spaces. This method enables precise and controlled generative outputs using Large Language Models (LLMs) and generative AI systems.

## Overview

This approach leverages mathematically-defined orthogonality to ensure conceptual independence among traits used for generative AI inputs. Each trait exists as an independent dimension, resulting in controlled and innovative creative outputs.

## Quickstart Guide

Follow these steps to replicate the orthogonal prompt engineering methodology:

### Step 1: Define Mutually Independent Dimensions

Create two sets of 32 independent dimensions each:

- **Character Dimensions (C01–C32)**: Traits defining psychological and emotional states.
- **Story Dimensions (S01–S32)**: Traits defining narrative structures and events.

Ensure each trait is conceptually independent.

### Step 2: Sample a Vector from the Defined Space

Select specific traits from both sets (Character & Story) to create an initial prompt vector. Example:

- **Character**: Inner Turbulence, Emotional Inaccessibility, Nonlinear Intuition, etc.
- **Story**: Public Fall from Grace, Discovery of Hidden Power, Transformation Through Illness, etc.

### Step 3: Generate Creative Outputs

- **3a. Generate Style**: Combine selected Character and Story dimensions into a coherent style prompt.
- **3b. Generate Lyrics**: Further refine the prompt using the previously generated Style along with Character and Story traits.

Example structured prompt:

>"Compose an indie folk song characterized by acoustic instrumentation and soft vocals. The emotional tone should reflect melancholic introspection with subtle hopeful resilience."

### Step 4: Orthogonal Sampling and Exploration

- **Element-wise Opposites**: Initially, sample vectors orthogonal (opposite) to the original vector to explore immediate conceptual opposites.
- **Additional Orthogonal Sampling**: Request further vectors orthogonal to previous samples. Initial orthogonality is straightforward; subsequent orthogonality will require more nuanced exploration, producing intriguing results.

### Step 5: Iteration and Expansion

When exhausted, define 64 new dimensions orthogonal to all previous vectors, thus continually expanding your creative possibility space.

## Practical Usage

This approach can systematically explore new conceptual territories while maintaining clear creative intent. It's particularly effective for:

- **Music Production**: Crafting emotionally nuanced musical compositions.
- **Storytelling**: Structuring complex narratives and character developments.
- **Branding and Corporate Art**: Ensuring innovative yet cohesive brand expressions.

## Testing and Validation

While the theoretical model of orthogonality ensures independence, practical orthogonality should be validated through embedding techniques (e.g., GloVe embeddings) to confirm semantic independence.

## Copyright Protection

Because engineered prompts can precisely dictate generative outputs, this methodology supports potential copyright protections, ensuring creative work is legally and ethically safeguarded.

## Conclusion

This methodology opens the traditionally opaque "black box" of LLMs, providing transparent, controlled, and repeatable generative outputs. It represents prompt engineering in its truest sense, offering substantial advancements in creative precision and control.

Here's a clear, parameterized algorithm to systematically construct two orthogonal vector spaces, ensuring orthogonality through sequential construction. We'll discuss both methods briefly before providing the algorithm explicitly:

---

### **Two Possible Approaches:**

**1. Sequential Construction (from nothing):**  
- Start with an empty set and iteratively add vectors, ensuring at each step that the new vector is orthogonal to all previously added vectors.

**2. Parameterized Approach (N dimensions):**  
- Start by defining a vector space with dimension \( N \).
- Construct another space such that every vector in this new space is orthogonal (dot product = 0) to all vectors in the original space.

Both methods are valid, but the parameterized approach is typically preferred in computational practice due to clarity and explicit control over dimensionality.

Below is the parameterized approach clearly outlined:

---

### **Parameterized Orthogonal Vector Space Construction (Algorithm):**

**Inputs:**  
- A set of vectors \(A\), each of dimension \(N\), forming the basis of the first vector space.
- Desired dimensionality \(M\) of the second (orthogonal) vector space, where \(M \leq N\).

**Outputs:**  
- A set of vectors \(B\), each of dimension \(N\), forming the basis of a second vector space orthogonal to \(A\).

---

### **Algorithm Steps:**

**Step 1: Initialization**  
- Let vector set \(A = \{a_1, a_2, ..., a_k\}\), each \(a_i \in \mathbb{R}^N\).  
- Confirm vectors in \(A\) are linearly independent and form a valid basis.

**Step 2: Form Matrix Representation**  
- Construct matrix \(M_A\) whose rows are the vectors in \(A\):

\[
M_A = \begin{bmatrix}
a_{1,1} & a_{1,2} & \dots & a_{1,N} \\
a_{2,1} & a_{2,2} & \dots & a_{2,N} \\
\vdots & \vdots & \ddots & \vdots \\
a_{k,1} & a_{k,2} & \dots & a_{k,N}
\end{bmatrix}
\]

**Step 3: Compute Orthogonal Complement via SVD**  
- Compute the Singular Value Decomposition (SVD) of \(M_A\):

\[
M_A = U \Sigma V^T
\]

- The orthogonal complement is found from the null space of \(M_A\), represented by singular vectors in \(V\) corresponding to zero singular values.

**Step 4: Extract Orthogonal Complement Vectors**  
- Identify vectors from \(V\) corresponding to zero (or near-zero numerically) singular values; these vectors span the orthogonal complement space.

**Step 5: Form Orthogonal Vector Space \(B\)**  
- Select the first \(M\) vectors from the orthogonal complement to form your second vector space \(B\).

---

### **Python Implementation Example:**

Below is a practical Python implementation of this algorithm using NumPy:

```python
import numpy as np

def orthogonal_complement_space(vectors, M=None, tol=1e-10):
    # Form matrix from input vectors (rows)
    matrix_A = np.vstack(vectors)

    # Compute Singular Value Decomposition
    U, S, Vt = np.linalg.svd(matrix_A)

    # Identify vectors in the null space (orthogonal complement)
    null_space = Vt[S <= tol].T

    # If M is specified, limit dimensions
    if M is not None and null_space.shape[1] >= M:
        null_space = null_space[:, :M]
    elif M is not None:
        raise ValueError(f"Orthogonal complement has fewer than {M} dimensions.")

    return null_space.T  # Each row is a vector in the orthogonal complement

# Example usage:
vectors_A = [
    [1, 0, 0, 0],
    [0, 1, 0, 0]
]

# Construct orthogonal complement space B
vectors_B = orthogonal_complement_space(vectors_A)

print(\"Orthogonal Vector Space B:\")
print(vectors_B)

# Verify orthogonality
for a in vectors_A:
    for b in vectors_B:
        dot_product = np.dot(a, b)
        print(f\"Dot product: {dot_product:.2f}\")  # Should be near zero
```

---

### **Explanation of the Provided Code:**

- The function `orthogonal_complement_space` takes input vectors defining space \(A\).
- Uses SVD to find the null space (orthogonal complement), thus constructing space \(B\).
- Allows explicit parameterization with desired dimensionality \(M\).
- Verifies that resulting vectors are orthogonal to the original vectors.

---

### **Conclusion:**

This parameterized SVD-based approach provides a robust and mathematically rigorous method for explicitly constructing two orthogonal vector spaces, starting with a known set of vectors in space \(A\) and systematically generating a space \(B\) fully orthogonal to it.