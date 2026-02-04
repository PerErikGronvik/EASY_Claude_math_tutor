# Instructions for Claude AI Assistant

## Project Context

This is a mathematical concepts notebook project for university-level mathematics courses (Calculus 1-4, Statistics, AI, etc.). Students use Jupyter notebooks for interactive learning.

## Notebook Interaction Guidelines

### 1. Import Management

**Always keep imports organized at the top of notebooks:**
- When adding new functionality that requires a package, add the import to the top cell
- Don't create separate import cells - always update and rerun the first cell. This keeps imports centralized and organized.
- If a package is missing from the environment, add it to `missing_packages.md`
- Keep imports grouped logically (standard library, third-party, local)

Example:
```python
# Standard library
import math

# Third-party packages
import numpy as np
import matplotlib.pyplot as plt
import sympy as sp
```

### 2. Explaining Concepts (Q&A Format)

When a user asks a question about a mathematical concept:

1. **Start with the prompt:** Create a markdown cell with the user's question/prompt
2. **Explain step-by-step:** Alternate between markdown cells (explanations) and code cells (demonstrations)
3. **One concept at a time:** Only answer what was asked - don't continue to solutions or related topics
4. **Interactive learning:** Wait for the user to ask follow-up questions rather than assuming what they want next

**Structure:**
```
[Markdown Cell] - User's question/prompt
[Markdown Cell] - Explanation of concept
[Code Cell] - Code demonstration
[Markdown Cell] - Interpretation of results
[Code Cell] - Additional example if needed
```

### 3. Stay Focused

**DO:**
- Answer the specific question asked
- Provide clear, concise explanations
- Show working code examples
- Wait for user to guide the conversation

**DON'T:**
- Continue to full solutions unprompted
- Assume the user wants to know related concepts
- Over-explain beyond the question
- Jump ahead in the learning process

This is a **back-and-forth learning exercise** where the student drives the pace and direction.

## Example Interaction

**User asks:** "What is a partial derivative?"

**Response:**
[Cell 1 -imports]
```python 
import numpy as np
```

```markdown
[Cell 2 - Markdown]
## What is a partial derivative?
```

```markdown
[Cell 3 - Markdown]
A partial derivative measures how a multivariable function changes 
when we vary only one variable while keeping others constant.
```

```python
[Cell 1 - Update into code cell]
import sympy as sp
** rerun cell 1 to include sp **
```

```python
[Cell 3 - Code]
x, y = sp.symbols('x y')
f = x**2 + 3*x*y + y**2

# Partial derivative with respect to x
df_dx = sp.diff(f, x)
df_dx
```

```markdown
[Cell 4 - Markdown]
The partial derivative ∂f/∂x = 2x + 3y shows how f changes 
as x changes (treating y as constant).
```

**STOP HERE** - Wait for user's next question rather than continuing to explain ∂f/∂y or applications.
