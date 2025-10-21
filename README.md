# Indian Equity Value Investment Stock Analyzer (n8n)
**Indian-Equity-Investment-Stock-Analyzer** is an automated workflow, purpose-built for value investing in the Indian stock market, leveraging the n8n automation platform. This project focuses on robust, data-driven stock analysis—grounded in fundamentals inspired by the "principles of Benjamin Graham, Philip Fisher, Peter Lynch, Mohnish Pabrai, and Joel Greenblatt." investment philosophy—strictly excluding speculation in favor of proven, ethical, and evidence-based decision-making.

## 4c8 Project Overview
This workflow fetches live stock data from NSE, processes multiple key value indicators, and uses an OpenAI GPT-4 Turbo agent to deliver insightful, readable investment analysis. Every step is recorded and displayed with transparent logs, execution metrics, and clear AI outputmaking sophisticated analysis accessible to both technical and non-technical users.

- **Trigger & Automate:** Start the workflow with a simple chat command (e.g., "Analyze RELIANCE stock").
- **Data Collection:** Instantly pulls latest data from NSE.
- **Fundamental Logic:** Applies value investing models (not speculation)inspired by "Deep Root."
- **AI-Powered:** OpenAI agent (GPT-4 Turbo) interprets data and provides plain-English summary, transparent logs, and run metrics.

## 680 Key Features
- **Automation:** End-to-end analysis powered by n8n workflow nodes for data, logic, and summaries.
- **Live Market Data:** Always operates on up-to-date NSE information.
- **Ethical Value Investing:** No guesswork, only fundamental indicators.
- **User-friendly Results:** Actionable insights, no jargon, full transparency.
- **Stepwise Clarity:** Visualization of setup, in-progress execution, and results (see screenshots).
- **Learning Showcase:** Transparent workflow logs, execution time, and token usage.

### Screenshots illustrate the workflow
- Workflow setup (automation nodes)
- Analysis execution (logs and agent output)
- Results/Output (AI summary and core metrics)

## 4a1 Learning & Aspiration
This project represents my commitment to ethics, transparent workflow automation, and powerful, readable analytics as I pursue a career in data analysis. By blending automation, value principles, and AI, I'm focused on helping usersand future employersaccess reliable, actionable market insights for confident investing.

**Tags:** n8n automation, Indian stock market, value investing, data analytics, OpenAI, NSE API, ethical investing, workflow automation

---

## How to use in n8n
To use this workflow, import IndianStockAnalyzer-workflow.json into your n8n account.

1) In n8n, go to Import from File and select the JSON.
2) Review environment variables (API keys, NSE endpoints) and credentials.
3) Activate the workflow and trigger it with a ticker symbol input.

## Screenshots and References
Screenshots are referenced from the /screenshots directory (stubs only, no actual images in repo):
- workflow-setup.png 4f7 Caption: Overall n8n workflow layout and node connections.
- node-details.png 4f7 Caption: Configuration panel for key nodes.
- execution-in-progress.png 4f7 Caption: Real-time execution view with logs.
- output-summary.png 4f7 Caption: Final AI summary with computed indicators.

## Node Documentation
See nodes.md for a table of nodes used, purpose, key parameters, and notes. Each node references the official n8n docs and relevant APIs.

- n8n Docs: https://docs.n8n.io/
- HTTP Request Node: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httpRequest/
- Code Node: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/
- AI/OpenAI Node: https://docs.n8n.io/integrations/builtin/ai-openai/

## Repository Structure
- IndianStockAnalyzer-workflow.json (stub, do not use in production)
- /screenshots (stub files and mini README)
- nodes.md (node table and descriptions)
- LICENSE (MIT or empty)
- .gitignore (Python/Node standard patterns)
- CONTRIBUTING.md (how to contribute)
- CHANGELOG.md (initial version notes)

## Disclaimers
- No actual images or workflow JSON are included; only placeholders/stubs are provided.
- This is an educational, non-financial-advice project. Always do your own research (DYOR).
