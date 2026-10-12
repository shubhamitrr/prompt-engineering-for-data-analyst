# Week 8 — Advanced Prompting

## 1. Introduction

Advanced prompting techniques help AI solve complex problems, explore different solutions, improve accuracy, and generate structured outputs.

## 2. Role Prompting

Role prompting assigns a specific role to the AI.

**Example:**

```text
Act as a senior data analyst.
Explain the sales performance of an e-commerce business.
```

**Benefit:** The response becomes more focused on the selected role.

## 3. Context and Constraints

Context provides background information, while constraints define the rules and limitations.

**Example:**

```text
Context: I am analyzing monthly sales data.

Task: Identify the top-performing product categories.

Constraints:
- Use only the provided data.
- Do not invent missing values.
- Keep the explanation simple.
```

**Benefit:** Improves relevance and reduces unwanted output.

## 4. Prompt Chaining

Prompt chaining divides a complex task into smaller prompts. The output of one step becomes the input for the next step.

**Example:**

1. Clean the sales dataset.
2. Perform exploratory data analysis.
3. Identify important trends.
4. Generate business recommendations.

**Benefit:** Makes complex tasks easier to manage and verify.

## 5. ReAct Prompting

ReAct stands for Reasoning and Acting. It combines reasoning with actions, such as searching information or running a tool, and uses the observations to continue the task.

**Example:**

```text
Task: Analyze the provided sales report.

1. Identify the required information.
2. Use an available tool to retrieve the report.
3. Examine the returned data.
4. Calculate important metrics.
5. Present findings with evidence.
```

**Benefit:** Useful for tasks that require tools or multiple steps.

**Note:** The system must have access to the required tools and permissions.

## 6. Tree of Thoughts

Tree of Thoughts explores multiple possible approaches before selecting a suitable solution.

**Example:**

```text
Suggest three approaches for reducing customer churn.
Compare each approach based on cost, impact, and difficulty.
Recommend the most suitable approach and explain why.
```

**Benefit:** Helps compare alternatives before making a decision.

## 7. Directional Stimulus Prompting

Directional stimulus prompting provides hints that guide the AI toward relevant aspects of a task.

**Example:**

```text
Analyze customer churn.

Focus on:
- Contract type
- Monthly charges
- Customer tenure
- Support complaints

Use the available data to identify patterns.
```

**Benefit:** Directs attention toward important information.

## 8. Iterative Prompt Development

Iterative development improves a prompt through repeated testing and refinement.

**Process:**

1. Write an initial prompt.
2. Review the output.
3. Identify missing details or errors.
4. Improve the instructions.
5. Test the revised prompt.
6. Verify whether the result improved.

**Initial Prompt:**

```text
Analyze sales.
```

**Improved Prompt:**

```text
Analyze the provided sales dataset.

Calculate total revenue, monthly revenue, and top-performing products.
Identify two important trends and provide three business recommendations.

Present the results using headings and a summary table.
```

## 9. Self-Consistency

Self-consistency compares multiple independently generated solutions to identify a consistent answer.

**Example:**

```text
Solve this numerical problem using three independent approaches.
Compare the results and verify the calculations.
If the answers differ, identify the source of disagreement.
```

**Benefit:** Can improve reliability for tasks with verifiable answers.

**Limitation:** Agreement between multiple AI outputs does not guarantee correctness.

## 10. Prompt Templates

Prompt templates use reusable structures with placeholders.

**Example:**

```text
Act as a [ROLE].

Context:
[BACKGROUND INFORMATION]

Task:
[REQUIRED TASK]

Constraints:
[IMPORTANT RULES]

Output Format:
[EXPECTED FORMAT]
```

**Benefit:** Saves time and keeps prompts consistent across projects.

## 11. Prompt Optimization

Prompt optimization means improving a prompt to obtain more accurate, relevant, and useful responses.

**Key Techniques:**

- Replace vague instructions with specific tasks.
- Add relevant context.
- Define constraints and assumptions.
- Specify the required output format.
- Include examples when useful.
- Test the prompt with different inputs.
- Verify results using reliable evidence.

## 12. Framework Comparison

| Technique | Main Purpose | Best Use Case |
|---|---|---|
| Role Prompting | Define the AI's role | Domain-specific answers |
| Prompt Chaining | Divide a complex task | Multi-stage analysis |
| ReAct | Combine reasoning and actions | Tool-assisted tasks |
| Tree of Thoughts | Compare possible approaches | Complex decisions |
| Directional Stimulus | Guide attention | Focused analysis |
| Iterative Development | Refine prompts | Improving output quality |
| Self-Consistency | Compare independent solutions | Verifiable reasoning tasks |
| Prompt Templates | Reuse prompt structures | Repeated workflows |
| Prompt Optimization | Improve prompt performance | Better and more consistent results |

## 13. Practical Data Analyst Exercise

**Task:** Analyze an e-commerce sales dataset.

**Prompt:**

```text
Act as an experienced data analyst.

Context:
I have an e-commerce dataset containing order dates,
products, categories, quantities, and sales values.

Tasks:
1. Identify missing values and duplicate records.
2. Summarize total sales and total orders.
3. Calculate monthly sales.
4. Identify the best-performing category.
5. Find important sales trends.
6. Recommend three business actions.

Constraints:
- Use only the supplied data.
- Do not invent missing values or results.
- Explain assumptions clearly.
- Verify calculations before reporting them.

Output:
1. Data quality summary
2. Key metrics table
3. Business insights
4. Recommendations
```

## 14. Best Practices

- Choose a technique according to the problem.
- Provide relevant context.
- Keep instructions specific.
- Use tools only when available and authorized.
- Break complex tasks into smaller steps.
- Compare alternatives when useful.
- Verify factual claims and calculations.
- Protect confidential information.
- Improve prompts based on test results.

## 15. Conclusion

Advanced prompting techniques help structure complex tasks, explore alternatives, use tools effectively, and improve AI output quality.

The best technique depends on the task. For reliable results, combine clear instructions, relevant context, appropriate tools, and independent verification.
