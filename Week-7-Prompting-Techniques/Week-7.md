# Week 7 — Prompting Techniques

## 1. Zero-Shot Prompting

### Definition

Zero-shot prompting is a technique where an AI model performs a task without receiving any examples.

### Example

Classify the following customer review:

> "The product quality is excellent."

Output:

**Positive**

### Key Point

Zero-shot prompting means **no examples are provided before the task**.

---

## 2. Few-Shot Prompting

### Definition

Few-shot prompting is a technique where an AI model receives a small number of examples before performing a similar task.

### Example

```text
Review: "The product is excellent."
Answer: Positive

Review: "The product quality is very poor."
Answer: Negative

Review: "The product works perfectly."
Answer:
```

Expected answer:

**Positive**

### Key Point

Few-shot prompting means **providing a few examples before the actual task**.

---

## 3. Chain of Thought

### Definition

Chain of Thought prompting encourages an AI model to solve a complex problem through logical intermediate steps before providing the final answer.

### Example

A product costs ₹800 and is sold for ₹1,000.

```text
Profit = 1000 - 800
Profit = 200

Profit Percentage = (200 / 800) × 100
Profit Percentage = 25%
```

Answer:

**25%**

### Data Analyst Example

Ask AI to calculate average sales by city and explain the calculation steps before providing the final result.

### Key Point

**Complex problem → Logical steps → Final answer**

---

## 4. Hallucinations

### Definition

AI hallucination occurs when an AI model generates incorrect, unsupported, or invented information.

### Example

Suppose a dataset does not contain an `Age` column.

If the AI says:

> "The average customer age is 32 years."

This is a hallucination because the required data was not available.

### How to Reduce Hallucinations

- Use only the provided data.
- Do not invent values.
- Avoid unsupported assumptions.
- Clearly mention missing information.
- Verify calculations.

### Key Point

**Hallucination = Incorrect or unsupported AI-generated information**

---

## 5. Logic Problem Lab

### Definition

A Logic Problem Lab is a practical exercise where AI is used to solve logical and reasoning problems.

### Common Examples

- Number series
- Logical puzzles
- Ranking problems
- Pattern identification
- Data-based reasoning

### Example

A is taller than B.

B is taller than C.

Therefore:

**A > B > C**

Answer:

**C is the shortest.**

### Data Analyst Example

IT has more employees than HR.

Sales has fewer employees than HR.

Therefore:

**IT > HR > Sales**

Answer:

**Sales has the fewest employees.**

### Key Point

**Logic Problem Lab = AI-assisted logical problem solving**

---

## 6. Prompt Verification

### Definition

Prompt verification is the process of checking whether an AI-generated answer is accurate, complete, relevant, and supported by the available information.

### Important Checks

- Data accuracy
- Calculations
- Missing information
- Assumptions
- Invented values
- Relevance

### Example

```text
Calculate the average salary of the employees.

Verify the calculation using the provided data before giving the final answer.
```

### Verification Process

**AI Answer → Check Data → Verify Calculation → Identify Errors → Final Answer**

### Key Point

**Prompt Verification = Checking AI output before using it**

---

## 7. Prompt Improvement

### Definition

Prompt improvement is the process of modifying a prompt to make it clearer, more specific, reliable, and effective.

### Weak Prompt

```text
Analyze my sales data.
```

### Problems

- The task is unclear.
- The expected output is not defined.
- No constraints are provided.
- No verification instructions are provided.

### Improved Prompt

```text
You are a Senior Data Analyst.

Analyze the provided sales dataset and identify the top 5 products by total sales.

Use only the provided data.
Do not invent values.
Verify all calculations.

Output:
1. A results table
2. Three key business insights
```

### Key Point

**Prompt Improvement = Weak Prompt → Clear and effective prompt**

---

## 8. Analytical Prompting

### Definition

Analytical prompting is the practice of designing prompts that help AI analyze data, calculate metrics, identify patterns, and generate useful insights.

### Common Analytical Tasks

- Calculate totals
- Calculate averages
- Find top and bottom records
- Identify trends
- Compare categories
- Identify patterns
- Generate business insights

### Example

Suppose a sales dataset contains:

`Product, City, Sales, Profit, Quantity`

Prompt:

```text
You are a Senior Data Analyst.

Analyze the sales dataset and identify the top 5 cities by total sales.

Calculate the average profit for each city.

Use only the provided data.
Do not invent values.
Verify all calculations.

Output:
1. A results table
2. Three business insights
```

### Key Point

**Analytical Prompting = AI + Data Analysis + Clear Instructions**

---

# Week 7 Summary

The major topics covered in Week 7 are:

1. Zero-Shot Prompting
2. Few-Shot Prompting
3. Chain of Thought
4. Hallucinations
5. Logic Problem Lab
6. Prompt Verification
7. Prompt Improvement
8. Analytical Prompting

## Final Takeaway

Effective prompting combines:

**Clear Instructions + Examples + Constraints + Verification + Analysis**

These techniques help create reliable and useful AI-assisted workflows for data analysis.
