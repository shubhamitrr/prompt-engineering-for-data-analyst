***# Week 7 — Prompting Techniques***



***## 1. Zero-Shot Prompting***



***### Definition***



***Zero-shot prompting is a technique where an AI model is asked to perform a task without being given any examples.***



***### Example***



***> Classify the following customer review as Positive, Negative, or Neutral:***

***>***

***> "The product quality is excellent."***



***No example is provided, so this is a \*\*zero-shot prompt\*\*.***



***### Data Analyst Example***



***> Find the top 5 products by sales from the provided dataset.***



***### Key Point***



***\*\*Zero-shot = No examples + Direct task\*\****



***---***



***## 2. Few-Shot Prompting***



***### Definition***



***Few-shot prompting is a technique where an AI model is provided with a small number of examples before being asked to perform a similar task.***



***### Example***



***> Classify customer reviews as Positive or Negative.***

***>***

***> \*\*Example 1:\*\****  

***> Review: "The product is excellent."***  

***> Answer: Positive***

***>***

***> \*\*Example 2:\*\****  

***> Review: "The product quality is very poor."***  

***> Answer: Negative***

***>***

***> \*\*Now classify:\*\****  

***> Review: "The product works perfectly."***



***Expected answer:***



***\*\*Positive\*\****



***### Data Analyst Example***



***> \*\*Example 1:\*\****  

***> Sales = 10,000, Profit = 2,000***  

***> Profit Margin = 20%***

***>***

***> \*\*Example 2:\*\****  

***> Sales = 5,000, Profit = 500***  

***> Profit Margin = 10%***

***>***

***> \*\*Now calculate:\*\****  

***> Sales = 8,000, Profit = 1,600***



***### Key Point***



***\*\*Few-shot = Few examples + New task\*\****



***---***



***## 3. Chain of Thought***



***### Definition***



***Chain of Thought prompting is a technique that encourages an AI model to solve a complex problem through intermediate reasoning steps before producing a final answer.***



***### Example***



***> A product costs ₹800 and is sold for ₹1,000. Calculate the profit percentage. Work through the calculation step by step and provide the final answer.***



***Calculation:***



***Profit = ₹1,000 − ₹800 = ₹200***



***Profit Percentage = (₹200 / ₹800) × 100***



***Answer = \*\*25%\*\****



***### Data Analyst Example***



***> Calculate the average sales for each city. Group the records by city, calculate the required values, verify the calculation, and provide the final result.***



***### Key Point***



***\*\*Chain of Thought = Complex problem → Step-by-step reasoning → Final answer\*\****



***---***



***## 4. Hallucinations***



***### Definition***



***AI hallucination occurs when an AI model generates information that is incorrect, unsupported by the provided data, or presented as a fact without sufficient evidence.***



***### Example***



***Suppose a dataset does not contain an Age column.***



***> Find the average age of customers.***



***If the AI responds:***



***> The average customer age is 32 years.***



***This is a hallucination because the required data was not available.***



***### How to Reduce Hallucinations***



***Use clear instructions such as:***



***- Use only the provided data.***

***- Do not invent values.***

***- Do not make unsupported assumptions.***

***- If information is missing, clearly state that it is unavailable.***

***- Verify calculations before providing the final answer.***



***### Key Point***



***\*\*Hallucination = Unsupported or incorrect AI-generated information\*\****



***---***



***## 5. Logic Problem Lab***



***### Definition***



***A Logic Problem Lab is a practical exercise where AI is used to solve reasoning and logical problems through clear and structured prompts.***



***### Common Examples***



***- Number series***

***- Logical puzzles***

***- Ranking problems***

***- Pattern identification***

***- Data-based reasoning***



***### Example***



***> A is taller than B.***  

***> B is taller than C.***  

***> Who is the shortest?***



***Logical relationship:***



***\*\*A > B > C\*\****



***Answer:***



***\*\*C is the shortest.\*\****



***### Data Analyst Example***



***> IT has more employees than HR.***  

***> Sales has fewer employees than HR.***  

***> Which department has the fewest employees?***



***Logical relationship:***



***\*\*IT > HR > Sales\*\****



***Answer:***



***\*\*Sales\*\****



***### Key Point***



***\*\*Logic Problem Lab = AI-assisted logical problem solving\*\****



***---***



***## 6. Prompt Verification***



***### Definition***



***Prompt verification is the process of checking whether an AI-generated answer is accurate, complete, relevant, and supported by the provided information.***



***### Why Verification Matters***



***AI-generated outputs should not always be accepted without checking them.***



***Important checks include:***



***- Calculations***

***- Data accuracy***

***- Missing information***

***- Assumptions***

***- Invented values***

***- Relevance***



***### Example***



***> Calculate the average salary of the employees and verify the calculation using the provided data before giving the final answer.***



***### Verification Process***



***\*\*AI Answer → Check Data → Verify Calculation → Identify Errors → Final Answer\*\****



***### Key Point***



***\*\*Prompt Verification = Checking AI output for accuracy and reliability\*\****



***---***



***## 7. Prompt Improvement***



***### Definition***



***Prompt improvement is the process of modifying a prompt to make it clearer, more specific, reliable, and effective.***



***### Weak Prompt***



***> Analyze my sales data.***



***### Problems***



***- The task is unclear.***

***- The required output is not defined.***

***- No constraints are provided.***

***- No verification instruction is provided.***



***### Improved Prompt***



***> You are a Senior Data Analyst.***

***>***

***> Analyze the provided sales dataset and identify the top 5 products by total sales.***

***>***

***> Use only the provided data and do not invent values.***

***>***

***> Verify the calculations before giving the final answer.***

***>***

***> Show the results in a table and provide 3 key business insights.***



***### Key Point***



***\*\*Prompt Improvement = Weak Prompt → Clear and effective prompt\*\****



***---***



***## 8. Analytical Prompting***



***### Definition***



***Analytical prompting is the practice of designing prompts that help AI analyze data, identify patterns, calculate metrics, and generate useful insights.***



***### Common Analytical Tasks***



***- Calculate totals***

***- Calculate averages***

***- Find top or bottom records***

***- Identify trends***

***- Compare categories***

***- Identify patterns***

***- Generate business insights***



***### Example***



***Suppose a sales dataset contains:***



***`Product, City, Sales, Profit, Quantity`***



***Prompt:***



***> You are a Senior Data Analyst.***

***>***

***> Analyze the sales dataset and identify the top 5 cities by total sales.***

***>***

***> Calculate the average profit for each city.***

***>***

***> Use only the provided data.***

***>***

***> Verify all calculations before giving the final answer.***

***>***

***> Show the results in a table and provide 3 business insights.***



***### Key Point***



***\*\*Analytical Prompting = AI + Data Analysis + Clear Instructions\*\****



***---***



***# Week 7 Summary***



***The major topics covered in Week 7 are:***



***1. Zero-Shot Prompting***

***2. Few-Shot Prompting***

***3. Chain of Thought***

***4. Hallucinations***

***5. Logic Problem Lab***

***6. Prompt Verification***

***7. Prompt Improvement***

***8. Analytical Prompting***



***### Final Takeaway***



***Effective prompting involves:***



***\*\*Clear Instructions + Examples + Constraints + Verification + Analysis\*\****



***These techniques help create more reliable and useful AI-assisted workflows for data analysis.***

