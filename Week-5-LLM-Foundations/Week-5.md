***# Week 5 — LLM Foundations***



***## 1. Course Introduction \& Syllabus***



***### Definition***



***A course introduction explains what you will learn, why you are learning it, and how the course is structured.***



***### Topics Covered***



***- LLMs***

***- Generative AI***

***- Prompt Engineering***

***- RCTNO Framework***

***- Zero-shot and Few-shot Prompting***

***- Advanced Prompting Techniques***

***- RAG***

***- AI Automation***

***- AI Tools for Data Analysts***



***### Example***



***Instead of asking:***



***> Analyze this data.***



***A better prompt is:***



***> You are a Data Analyst. Analyze this sales dataset, identify the top 5 products by revenue, explain the main trends, and present the result in a table.***



***---***



***## 2. AI "Boss" Analogy***



***### Definition***



***The AI "Boss" Analogy is a way of understanding AI as an employee who follows the instructions given by a human.***



***### Explanation***



***The human acts as the boss and AI acts as an assistant. Clear instructions help AI produce more useful results.***



***### Example***



***Poor prompt:***



***> Analyze this data.***



***Better prompt:***



***> You are a Data Analyst. Analyze this sales data and find the top 5 products by sales. Show the result in a table and provide 3 key insights.***



***### Key Point***



***Clear Prompt → Better Output***



***---***



***## 3. What is LLM?***



***### Definition***



***LLM (Large Language Model) is an AI model trained on a large amount of text and data to understand and generate human-like language.***



***### Explanation***



***An LLM learns patterns, relationships, and structures from large amounts of training data. It can then generate responses based on a user's prompt.***



***### Example***



***User:***



***> Explain SQL JOIN in simple words.***



***LLM:***



***> SQL JOIN is used to combine data from two or more tables using a related column.***



***### Examples of LLMs***



***- GPT***

***- Gemini***

***- Claude***

***- Llama***



***### Key Point***



***LLM = AI model that understands and generates human-like text.***



***---***



***## 4. Discriminative vs Generative AI***



***### Definition***



***Discriminative AI is an AI system that learns to classify or predict outcomes from existing data.***



***Generative AI is an AI system that learns patterns from data and can create new content such as text, images, audio, or code.***



***### Explanation***



***Discriminative AI mainly decides or classifies.***



***Generative AI creates new content.***



***### Example — Discriminative AI***



***An AI system receives an email and predicts:***



***> Spam / Not Spam***



***### Example — Generative AI***



***User:***



***> Write a professional email for a job application.***



***AI generates a new email.***



***### Key Difference***



***Discriminative AI → Classify or Predict***



***Generative AI → Create New Content***



***---***



***## 5. AI Evolution***



***### Definition***



***AI Evolution refers to the development of Artificial Intelligence from early rule-based systems to modern AI models such as neural networks, transformers, and LLMs.***



***### Explanation***



***AI developed gradually through different stages.***



***### Major Stages***



***1. Rule-Based Systems***

***2. Machine Learning***

***3. Neural Networks***

***4. RNN***

***5. LSTM***

***6. Transformers***

***7. LLMs***



***### Example***



***Early AI:***



***> If temperature > 30°C → "Hot"***



***Machine Learning:***



***> Learn patterns from historical weather data to predict temperature.***



***Modern AI:***



***> Explain why the temperature is increasing in this city.***



***An LLM can generate a natural-language response.***



***### Key Point***



***AI Evolution = From predefined rules to systems that can learn patterns and generate content.***



***---***



***## 6. RNN***



***### Definition***



***RNN (Recurrent Neural Network) is a type of neural network designed to process sequential data by using information from previous steps.***



***### Explanation***



***RNN uses information from previous steps while processing the current input. It is useful when the order of information is important.***



***### Common Applications***



***- Text***

***- Speech***

***- Time Series***

***- Stock Prices***



***### Example***



***For the sentence:***



***> I am learning Python.***



***An RNN processes the words as a sequence:***



***I → am → learning → Python***



***Previous information can influence the processing of the current word.***



***### Limitation***



***RNNs can have difficulty remembering important information over very long sequences.***



***This limitation led to models such as LSTM.***



***### Key Point***



***RNN → Processes sequential data using previous information.***



***---***



***## 7. LSTM***



***### Definition***



***LSTM (Long Short-Term Memory) is a type of recurrent neural network designed to remember important information for a longer period of time.***



***### Explanation***



***LSTM is an improved type of RNN that uses a memory mechanism to decide what information should be kept, forgotten, or added.***



***### Example***



***Sentence:***



***> Shubham studied Python for 6 months. He used it to build a data analysis project.***



***LSTM can use the earlier information about Shubham and Python when processing the later part of the sentence.***



***### RNN vs LSTM***



***| RNN | LSTM |***

***|---|---|***

***| Basic sequential model | Improved sequential model |***

***| Limited long-term memory | Better long-term memory |***

***| Can forget older information | Better at retaining important information |***

***| Simpler | More complex |***



***### Key Point***



***LSTM → RNN with better long-term memory.***



***---***



***## 8. Transformers***



***### Definition***



***A Transformer is a neural network architecture that processes sequences using attention mechanisms, allowing it to understand relationships between different parts of the input.***



***### Explanation***



***Transformers can analyze relationships between words or tokens using attention. Unlike traditional RNN-based approaches, Transformers can process many parts of a sequence more efficiently in parallel.***



***### Example***



***Sentence:***



***> The student went to the bank because he needed money.***



***A Transformer can use attention to understand the relationship between "he" and "student" and the meaning of "bank" from the surrounding context.***



***### Examples***



***Many modern AI models use Transformer-based architectures, including:***



***- GPT***

***- BERT***

***- Gemini***

***- Llama***



***### Key Point***



***Transformer → Uses attention to understand relationships between different parts of the input.***



***---***



***## 9. Attention Mechanism***



***### Definition***



***Attention Mechanism is a technique that allows an AI model to focus on the most relevant parts of the input when processing information.***



***### Explanation***



***Attention helps the model determine which words or tokens are more important for understanding the current context.***



***### Example***



***Sentence:***



***> I went to the bank to deposit money.***



***The words "deposit" and "money" provide important context for understanding that "bank" refers to a financial institution.***



***Attention helps the model consider these relationships.***



***### Why Attention Is Important***



***- Understands context***

***- Connects related words***

***- Helps process long sequences***

***- Identifies relevant information***



***### Key Point***



***Attention → Focuses on relevant information to better understand context.***



***---***



***## 10. Tokens \& Cost Analysis***



***### Definition***



***A token is a small unit of text that an AI model processes. Tokens can be words, parts of words, punctuation marks, or other text units.***



***### Explanation***



***AI models process text as tokens rather than treating an entire sentence as one single unit.***



***A token is not always equal to one complete word.***



***### Example***



***Text:***



***> I love Python.***



***This text is converted into multiple tokens before being processed by the model.***



***### Token Usage***



***Token usage can include:***



***- Input tokens***

***- Output tokens***



***Total token usage depends on the amount of text processed.***



***### Cost Analysis***



***Many AI APIs charge based on the number of tokens processed.***



***More tokens → More processing → Potentially higher cost***



***### Example***



***If an API charges a specific price per million tokens, processing more tokens will increase the API cost.***



***### Key Point***



***Token = A small unit of text processed by an AI model.***



***More token usage can mean higher API cost.***



***---***



***## 11. Context Windows \& Memory Limits***



***### Definition***



***A context window is the maximum amount of information an AI model can process at one time.***



***### Explanation***



***An AI model can only consider a limited amount of information within a single context. The size of this limit depends on the model.***



***### Example***



***Suppose a user wants an AI model to analyze a very large document.***



***If the document is larger than the model's available context window, the entire document may not fit into one request.***



***The document can be:***



***- Split into smaller chunks***

***- Summarized***

***- Processed separately***

***- Used with a RAG system***



***### Context Window vs Memory***



***\*\*Context Window:\*\****



***The information the model can process within the current interaction.***



***\*\*Memory:\*\****



***Information that a system may store and use across interactions, depending on the AI product and its settings.***



***These are not the same thing.***



***### Why It Matters for Data Analysts***



***Large datasets, long SQL queries, reports, and multiple documents can create context limitations.***



***Techniques such as chunking, summarization, and RAG can help manage large amounts of information.***



***### Key Point***



***Context Window → The amount of information an AI model can handle at one time.***



***Memory → Information that may be stored and used beyond the current context.***

