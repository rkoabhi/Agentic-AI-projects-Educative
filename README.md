AI Multi-Agent Research Assistant



This project is a small experiment where I built a multi-agent AI system that can take a research idea and turn it into a structured report.



The idea was to simulate how research actually happens:



\* start with a vague idea

\* refine it

\* find relevant papers

\* extract insights

\* organize everything into a report

\* identify gaps and future directions







What this project does



Given an input like:



AI for healthcare



The system will:



1\. Refine it into a more specific research topic

2\. Search for relevant research papers using the arXiv API

3\. Summarize key insights from those papers

4\. Generate a structured report

5\. Suggest research gaps and possible future work





Agents used in the system



I created multiple agents, each with a specific role:



Topic Agent → refines the research idea

Paper Agent → fetches papers from arXiv

Insight Agent → extracts key points

Report Agent → creates a structured report

Gap Agent → identifies missing areas and future directions



There is also a User Proxy Agent, which allows manual approval before continuing.

You can type:



APPROVE → continue

DISAPPROVE → refine the topic again







How the workflow works



The agents run in sequence like this:



User Input

→ Topic Agent

→ User Approval

→ Paper Agent

→ Insight Agent

→ Report Agent

→ Gap Agent

→ Final Output



The system automatically stops when the final report is generated.







Tech stack



\* Python

\* AutoGen (AgentChat)

\* OpenAI API

\* arXiv API

\* Async execution







How to run this project



1\. Clone the repository:

&#x20;  git clone https://github.com/YOUR\_USERNAME/ai-research-agent.git



2\. Go into the folder:

&#x20;  cd ai-research-agent



3\. Install dependencies:

&#x20;  pip install -r requirements.txt



4\. Create a `.env` file and add your API key:

&#x20;  OPENAI\_API\_KEY=your\_api\_key\_here



5\. Open the notebook:

&#x20;  research.ipynb



6\. Run all cells and follow the prompts.





