# Indian Equity Value Investment Stock Analyzer (n8n)

**Indian-Equity-Investment-Stock-Analyzer** is an automated workflow, purpose-built for value investing in the Indian stock market, leveraging the n8n automation platform. This project focuses on robust, data-driven stock analysis—grounded in fundamentals inspired by the "principles of Benjamin Graham, Philip Fisher, Peter Lynch, Mohnish Pabrai, and Joel Greenblatt." investment philosophy—strictly excluding speculation in favor of proven, ethical, and evidence-based decision-making.

## Project Overview

This workflow fetches live stock data from NSE, processes multiple key value indicators, and uses an OpenAI GPT-4 Turbo agent to deliver insightful, readable investment analysis. Every step is recorded and displayed with transparent logs, execution metrics, and clear AI output—making sophisticated analysis accessible to both technical and non-technical users.

### Complete Workflow Architecture

![Complete Workflow](screenshots/screenshots/00_complete_workflow.png)
*Figure 1: Complete n8n workflow showing all nodes and their connections for Indian stock analysis*

- **Trigger & Automate:** Start the workflow with a simple chat command (e.g., "Analyze RELIANCE stock").
- **Data Collection:** Instantly pulls latest data from NSE.
- **Fundamental Logic:** Applies value investing models (not speculation) inspired by "Deep Root."
- **AI-Powered:** OpenAI agent (GPT-4 Turbo) interprets data and provides plain-English summary, transparent logs, and run metrics.

## Key Features

- **Automation:** End-to-end analysis powered by n8n workflow nodes for data, logic, and summaries.
- **Live Market Data:** Always operates on up-to-date NSE information.
- **Ethical Value Investing:** No guesswork, only fundamental indicators.
- **User-friendly Results:** Actionable insights, no jargon, full transparency.
- **Stepwise Clarity:** Visualization of setup, in-progress execution, and results (see screenshots).
- **Learning Showcase:** Transparent workflow logs, execution time, and token usage.

## Learning & Aspiration

This project represents my commitment to ethics, transparent workflow automation, and powerful, readable analytics as I pursue a career in data analysis. By blending automation, value principles, and AI, I'm focused on helping users—and future employers—access reliable, actionable market insights for confident investing.

**Tags:** n8n automation, Indian stock market, value investing, data analytics, OpenAI, NSE API, ethical investing, workflow automation

---

## How to use in n8n

To use this workflow, import IndianStockAnalyzer-workflow.json into your n8n account.

1) In n8n, go to Import from File and select the JSON.
2) Review environment variables (API keys, NSE endpoints) and credentials.
3) Activate the workflow and trigger it with a ticker symbol input.

![Trigger Node Configuration](screenshots/screenshots/01_trigger_node.png)
*Figure 2: Chat trigger node configuration for initiating stock analysis*

## Workflow Components

### 1. Workflow Configuration

![Workflow Config](screenshots/screenshots/02_workflow_config.png)
*Figure 3: Workflow settings and execution parameters*

The workflow is configured with proper error handling, execution timeout, and logging settings to ensure reliable operation.

### 2. NSE Data Fetching

![NSE API Node](screenshots/screenshots/03_nse_api_node.png)
*Figure 4: NSE API integration node for fetching live market data*

This node connects to the NSE API to retrieve real-time stock information including price, volume, and fundamental metrics.

### 3. Analysis Agent

![Analysis Agent](screenshots/screenshots/04_analysis_agent.png)
*Figure 5: AI analysis agent configuration and processing logic*

The analysis agent processes the raw market data using value investing principles and prepares it for AI interpretation.

### 4. GPT-4 Summarizer

![GPT-4 Summarizer](screenshots/screenshots/05_gpt4_summarizer.png)
*Figure 6: OpenAI GPT-4 node for generating investment insights*

The GPT-4 Turbo model generates clear, actionable investment insights based on the processed fundamental data.

### 5. Supporting Nodes

![Supporting Nodes](screenshots/screenshots/06_supporting_nodes.png)
*Figure 7: Helper nodes for data transformation and formatting*

Additional nodes handle data transformation, formatting, and output preparation.

### 6. Workflow Execution

![Workflow Execution](screenshots/screenshots/workflow_execution.png)
*Figure 8: Live workflow execution showing real-time processing and results*

Watch the workflow in action as it processes stock data and generates insights in real-time.

## Screenshots and Visual Documentation

For detailed visual documentation of each workflow component, see the [screenshots README](screenshots/README.md) which provides:

1. **Complete Workflow Overview** - Full canvas view of all nodes and connections
2. **Trigger Node** - Chat interface setup for user interaction
3. **Workflow Configuration** - Settings, parameters, and execution options
4. **NSE API Node** - Live data fetching configuration
5. **Analysis Agent** - Value investing logic implementation
6. **GPT-4 Summarizer** - AI-powered insight generation
7. **Supporting Nodes** - Data transformation and formatting helpers
8. **Workflow Execution** - Real-time processing and output display

## Node Documentation

See [nodes.md](nodes.md) for a table of nodes used, purpose, key parameters, and notes. Each node references the official n8n docs and relevant APIs.

- n8n Docs: https://docs.n8n.io/
- HTTP Request Node: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httpRequest/
- Code Node: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/
- AI/OpenAI Node: https://docs.n8n.io/integrations/builtin/ai-openai/

## Repository Structure

- IndianStockAnalyzer-workflow.json (stub, do not use in production)
- /screenshots (visual documentation of workflow)
  - /screenshots (actual image files)
  - README.md (detailed description of each screenshot)
- nodes.md (node table and descriptions)
- LICENSE (MIT or empty)
- .gitignore (Python/Node standard patterns)
- CONTRIBUTING.md (how to contribute)
- CHANGELOG.md (initial version notes)

## Disclaimers

- Screenshots document the workflow structure and configuration; actual implementation may vary
- This is an educational, non-financial-advice project. Always do your own research (DYOR).
- Requires proper API credentials and n8n setup for full functionality
