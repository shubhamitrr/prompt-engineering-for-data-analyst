# Week 3 — Advanced Prompting

## 1. Zero-shot vs Few-shot Prompting

### Zero-shot Prompting

Zero-shot means giving a task to AI **without providing any example**.

**Example:**

> Find the top 5 products by sales from this dataset.

### Few-shot Prompting

Few-shot means giving AI **a few examples** so it understands the expected pattern.

**Example:**

> Low Sales → Needs Attention
> High Sales → Good Performance
>
> Classify the following products using the same pattern.

### Easy Trick

* Zero-shot = 0 examples
* Few-shot = Few examples

---

## 2. Structured Output

Structured output means asking AI to return the answer in a **specific format**.

Common formats:

* Table
* Bullet points
* Numbered list
* JSON
* Python code
* SQL query

**Example Prompt:**

> Analyze the sales data and return the result in a table with Product, Total Sales, and Total Profit columns.

### Easy Trick

**Structured Output = Answer kis format mein chahiye?**

---

## 3. Prompt Templates

A Prompt Template is a **reusable prompt structure** where some information can be changed.

**Example:**

```text
You are a Data Analyst.

Analyze the [DATASET NAME] dataset.

Focus on these columns:
[COLUMNS]

Find:
[TASK]

Return the result as:
[OUTPUT FORMAT]
```

Here, `[DATASET NAME]`, `[COLUMNS]`, `[TASK]`, and `[OUTPUT FORMAT]` can change.

### Benefit

The same prompt can be reused for different datasets and tasks.

### Easy Trick

**Fixed Prompt + Changeable Information = Prompt Template**

---

## 4. Step-by-step Reasoning Requests

For complex tasks, we can ask AI to break the task into smaller steps.

**Example:**

> Analyze this sales dataset step by step:
>
> 1. Check missing values.
> 2. Check duplicate rows.
> 3. Calculate total sales and profit.
> 4. Find the top 5 products.
> 5. Identify important business insights.

This makes the task easier to understand and organize.

**Important:** Instead of asking for private chain-of-thought, ask for the **steps, calculations, assumptions, and final result** that are useful for checking the work.

### Easy Trick

**Complex Task → Small Steps → Final Result**

---

## 5. Self-check / Verification Prompts

Self-check means asking AI to **review its answer before giving the final result**.

**Example:**

> Write a MySQL query to find the top 5 employees by salary. Check the SQL syntax and requirements before providing the final query.

For DAX:

> Create a Profit Margin measure and verify that the formula handles division by zero correctly.

Useful instructions:

* Check for errors.
* Verify the calculation.
* Check SQL syntax.
* Confirm the requirements.
* Identify assumptions.
* Correct mistakes.

### Easy Trick

**Answer → Check → Correct → Final Answer**

---

## 6. Prompt Chaining

Prompt chaining means breaking a large task into **multiple connected prompts**.

The output of one prompt becomes the input for the next prompt.

### Example — Sales Analysis

**Prompt 1:**
Clean the sales dataset and handle missing values.

**Prompt 2:**
Using the cleaned dataset, perform EDA and find important patterns.

**Prompt 3:**
Using the EDA results, identify important business insights.

### Difference

**Step-by-step reasoning request:**
One prompt contains multiple steps.

**Prompt chaining:**
Multiple prompts are connected together.

### Easy Trick

**Prompt 1 → Output → Prompt 2 → Output → Prompt 3**

---

## 7. Context Management

### Context

Context is the information AI needs to properly understand a task.

**Example:**

> The dataset contains 5,000 customers.
> The `Churn` column contains Yes/No values.
> "Yes" means the customer left the company.

This information helps AI understand the dataset correctly.

### Context Management

Context management means deciding:

* What information should be provided?
* How much information is needed?
* Which information is relevant?
* Which unnecessary information should be removed?
* When should previous information be provided?

### Easy Difference

**Context = What information AI needs**

**Context Management = How we provide and manage that information**

### Easy Trick

**Relevant Context > More Context**

---

## 8. Handling Ambiguous Data Questions

Ambiguous means **unclear or confusing**.

### Example

> Find the best product.

This is unclear because "best" could mean:

* Highest Sales
* Highest Profit
* Highest Quantity
* Highest Rating

A good prompt should handle this ambiguity.

**Example:**

> If any part of my question is ambiguous, identify the ambiguity and state your assumption before proceeding. Do not silently make assumptions.

If clarification is not available, clearly mention the assumption.

**Example:**

> Assumption: I am considering the product with the highest Sales as the best product.

### Easy Trick

**Unclear Question → Identify Ambiguity → Ask/State Assumption → Proceed**

---

## 9. Hallucination Reduction

Hallucination occurs when AI provides **incorrect or unsupported information as if it were true**.

### Data Analyst Examples

AI might:

* Invent dataset values.
* Give an incorrect SQL query.
* Give a wrong Excel formula.
* Give an incorrect DAX measure.
* Calculate statistics incorrectly.
* Create unsupported business insights.

### How to Reduce Hallucinations

Tell AI to:

1. Use only the provided data.
2. Do not invent missing information.
3. Clearly state assumptions.
4. Say when information is unavailable.
5. Verify calculations.
6. Check the final answer.

**Example Prompt:**

> Use only the data provided. Do not invent values or information. If information is missing, clearly mention it. State any assumptions and verify calculations before providing the final answer.

### Easy Trick

**Don't Guess → Use Data → State Assumptions → Verify**

---

## 10. Reliable Analytical Prompts

A Reliable Analytical Prompt is designed to make AI analysis **clear, accurate, verifiable, and based on the provided data**.

### Main Components

A reliable prompt can include:

**Role + Context + Task + Constraints + Output Format + Verification**

### Example

> You are a Data Analyst.
> Analyze the provided sales dataset.
> First check missing values and duplicate rows.
> Calculate total Sales and Profit.
> Find the top 5 products by Sales.
> Identify products with negative Profit.
> Provide 5 important business insights.
> Use only the provided data.
> Do not invent information.
> State any assumptions.
> Verify calculations before giving the final answer.
> Return results using tables and bullet points.

### Easy Formula

**Reliable Prompt = Clear Task + Context + Rules + Output Format + Verification**

---

# Week 3 Summary

In Week 3, we learned advanced techniques for creating more reliable and reusable prompts.

| Topic                   | Main Idea                     |
| ----------------------- | ----------------------------- |
| Zero-shot               | No examples                   |
| Few-shot                | Few examples                  |
| Structured Output       | Specific answer format        |
| Prompt Templates        | Reusable prompt structure     |
| Step-by-step            | Break complex task into steps |
| Self-check              | Verify the answer             |
| Prompt Chaining         | Connect multiple prompts      |
| Context Management      | Manage relevant information   |
| Ambiguity Handling      | Identify unclear questions    |
| Hallucination Reduction | Reduce unsupported answers    |
| Reliable Prompts        | Clear + contextual + verified |

## Week 3 Key Formula

**Good Prompt → Clear Task → Relevant Context → Rules → Output Format → Verification**

## Data Analyst Application

These techniques can be used with:

* Excel
* SQL
* Python/Pandas
* Data Cleaning
* EDA
* Matplotlib/Seaborn
* Power BI
* DAX
* Business Analysis
* AI-assisted Data Analytics
