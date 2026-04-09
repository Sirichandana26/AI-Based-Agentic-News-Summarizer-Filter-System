# AI-Based-Agentic-News-Summarizer-Filter-System
AI-Based Agentic News Summarizer & Filter System

1. 🧠 Business Problem
In today’s digital world, users are exposed to a large volume of news from multiple sources. It becomes difficult to read all articles and identify which ones are truly important.
Most existing systems:
•	Provide excessive information 
•	Lack transparency in filtering 
•	Do not consider user preferences effectively 
👉 This leads to information overload and wasted time

2. 💡 Possible Solution
To solve this problem, we can build an intelligent system that:
•	Automatically collects news from reliable sources 
•	Uses AI to summarize content 
•	Evaluates importance based on context 
•	Filters and delivers only relevant news 
👉 This reduces unnecessary information and improves user experience

3. 🚀 Implemented Solution
We implemented an Agentic AI system using n8n that:
•	Fetches news using RSS feeds 
•	Summarizes news using an LLM (via OpenRouter API) 
•	Classifies news as IMPORTANT or NOT IMPORTANT 
•	Filters based on user preferences (e.g., Technology, AI) 
•	Sends only important news via email 
👉 The system follows:
Observe → Reason → Decide → Act

4. 🛠️ Tech Stack Used
•	n8n – Workflow automation 
•	OpenRouter API – LLM for summarization and decision-making 
•	RSS Feed – News data source 
•	Gmail Node – Sending notifications 

5. 🧩 Architecture Diagram
RSS Read → HTTP Request (AI) → IF Node → Gmail
Explanation:
•	RSS → Collects news 
•	AI → Summarizes and analyzes 
•	IF → Filters important news 
•	Gmail → Sends alerts 

6. ⚙️ How to Run in Local
1.	Install and start n8n (using Docker or npm) 
2.	Create a new workflow 
3.	Add nodes: 
o	RSS Read 
o	HTTP Request (OpenRouter API) 
o	IF Node 
o	Gmail (Send Message) 
4.	Configure API key in HTTP node 
5.	Execute workflow 
6.	Check email for output 

7. 📚 References and Resources Used
•	https://n8n.io 
•	https://openrouter.ai 
•	https://rss.nytimes.com 
•	LLM prompt engineering concepts

9. 🎥 Recording



9. 📸 Screenshots
Include:
  



11. 🧾 Proper Formatting and Alignment
•	Structured using headings and sections 
•	Clear separation of components 
•	Easy to read and understand 
•	Suitable for academic submission 

12. ⚠️ Problems Faced and Solutions
🔴 Problem 1: Gemini API quota exceeded
👉 Solution: Switched to OpenRouter API

🔴 Problem 2: JSON parsing errors
👉 Solution: Used proper RAW JSON format in HTTP node

🔴 Problem 3: Model not available
👉 Solution: Used openrouter/auto model

🔴 Problem 4: Incorrect API configuration
👉 Solution: Fixed headers and request format

🏁 Conclusion
This project demonstrates an Agentic AI system that intelligently processes and filters news based on relevance and user preferences. It reduces information overload and provides a practical real-world solution using automation and AI.

