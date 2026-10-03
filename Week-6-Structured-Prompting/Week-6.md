# Week 6 — Structured Prompting

## 1. RCTNO Framework

### Definition

RCTNO Framework is a structured prompting method that helps create clear and effective prompts using five elements: Role, Context, Task, Narrowing, and Output.

### Explanation

RCTNO helps us give clear instructions to AI.

- **R — Role:** Tell AI who it should act as.
- **C — Context:** Provide background information.
- **T — Task:** Tell AI what to do.
- **N — Narrowing:** Define rules and limitations.
- **O — Output:** Specify the required output format.

### Example

**Role:** You are a Data Analyst.

**Context:** I have a sales dataset containing Product, Sales, and Profit.

**Task:** Find the top 5 products by sales.

**Narrowing:** Use only the provided data.

**Output:** Show the result in a table with 3 key insights.

---

## 2. Role

### Definition

Role is the instruction that tells the AI who it should act as while answering a prompt.

### Explanation

Role tells AI which professional or expert perspective it should use.

### Example

> You are an experienced Data Analyst. Analyze this sales dataset and identify the top 5 products by sales.

### Key Point

**Role = Who should AI act as?**

---

## 3. Context

### Definition

Context is the background information that helps AI understand the situation, data, or problem before performing a task.

### Explanation

Context gives AI the necessary background information.

### Example

> I have a retail sales dataset containing Product, Sales, Quantity, Region, and Profit columns.

This information is the **Context**.

### Key Point

**Context = Background information.**

---

## 4. Task

### Definition

Task is the specific work or action that you want the AI to perform.

### Explanation

Task clearly tells AI what it needs to do.

### Example

> Find the top 5 products by total sales.

This sentence is the **Task**.

### Key Point

**Task = What should AI do?**

---

## 5. Narrowing / Constraints

### Definition

Narrowing or Constraints are rules and limitations that tell AI how the task should be performed.

### Explanation

Constraints control the AI's output and prevent unwanted assumptions.

### Example

- Use only the provided data.
- Do not invent values.
- Show only the top 5 results.
- Verify calculations before giving the final answer.

### Key Point

**Narrowing = Rules and limitations.**

---

## 6. Output Format

### Definition

Output Format tells AI how the final answer should be presented.

### Explanation

It specifies the structure in which we want the answer.

### Common Formats

- Table
- Bullet points
- Numbered list
- JSON
- SQL code
- Short paragraph

### Example

> Show the top 5 products in a table with Product Name and Total Sales columns.

### Key Point

**Output = How should the answer be presented?**

---

## 7. Structured Prompting

### Definition

Structured Prompting is the practice of organizing a prompt into clear sections so that AI can understand the instructions easily and produce a consistent output.

### Explanation

Instead of putting everything into one sentence, we organize the prompt into sections such as Role, Context, Task, Constraints, and Output.

### Example

**Role:** You are a Data Analyst.

**Context:** I have a retail sales dataset.

**Task:** Find the top 5 products by sales.

**Constraints:** Use only the provided data.

**Output:** Show the result in a table and provide 3 insights.

### Benefits

- Clear instructions
- Organized output
- Easier to reuse
- Fewer misunderstandings

### Key Point

**Structured Prompting = Organizing instructions into clear sections.**

---

## 8. Marketing Content Lab

### Definition

A Marketing Content Lab is a practical exercise where AI is used to create, improve, or analyze marketing content using structured prompts.

### Explanation

AI can help create:

- Instagram captions
- Product descriptions
- Advertisement copy
- Email subject lines
- Social media posts

### Example

**Role:** You are a Marketing Content Writer.

**Context:** We sell affordable wireless earbuds for college students.

**Task:** Create an Instagram caption.

**Narrowing:** Use simple English and keep it under 50 words.

**Output:** Give 3 caption options.

### Key Point

**Marketing Content Lab = Using structured prompts for marketing tasks.**

---

## 9. Cold Email Lab

### Definition

A Cold Email is an email sent to a person or company with whom you have no previous communication, usually for a professional purpose.

### Explanation

Cold emails can be used for:

- Job opportunities
- Internships
- Networking
- Business communication

### Example

**Role:** You are a professional career communication assistant.

**Context:** I am a B.Tech IT student looking for a Data Analyst internship.

**Task:** Write a cold email asking about Data Analyst internship opportunities.

**Narrowing:** Keep it under 120 words and use simple professional English.

**Output:** Provide a subject line and email body.

### Key Point

**Cold Email Lab = Using AI to create professional first-contact emails.**

---

## 10. Big Data Analysis Lab

### Definition

Big Data Analysis is the process of examining large and complex datasets to find patterns, trends, relationships, and useful insights.

### Explanation

AI can assist with:

- Finding patterns
- Identifying trends
- Summarizing data
- Identifying anomalies
- Generating business insights

### Example

**Role:** You are a Data Analyst.

**Context:** I have a large sales dataset containing customer, product, region, sales, and profit data.

**Task:** Identify major sales trends and low-performing regions.

**Narrowing:** Use only the provided data and clearly separate facts from assumptions.

**Output:** Give 5 key insights in bullet points and a summary table.

### Key Point

**Big Data Analysis Lab = Using AI-assisted analysis for large datasets.**

---

## Week 6 Summary

RCTNO Framework provides a structured way to create effective prompts:

**Role → Context → Task → Narrowing → Output**

Structured prompting helps AI understand instructions clearly and produce more relevant, consistent, and controlled results.

### Week 6 Key Takeaway

**Good Prompt = Clear Role + Relevant Context + Specific Task + Strong Constraints + Defined Output**
