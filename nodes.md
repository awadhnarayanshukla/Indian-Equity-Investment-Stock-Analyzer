# Node Descriptions

This document provides detailed descriptions of all nodes used in the Indian Equity Investment Stock Analyzer workflow. Each node plays a specific role in the automated stock analysis pipeline.

---

## Node List and Descriptions:

### 1. When Chat Message Received (Trigger Node)

**Role:** Serves as the entry point for the workflow. This trigger node activates when a user sends a chat message containing a stock symbol or company name, initiating the entire analysis pipeline automatically.

**Key Features:**
- Listens for incoming chat messages
- Parses user input to extract stock symbols
- Passes the extracted data to subsequent nodes
- Enables real-time, on-demand stock analysis

**Screenshot Reference:** See `screenshots/01_trigger_node.png` for the trigger node configuration and message handling setup.

---

### 2. Workflow Configuration (Manual Node)

**Role:** Provides manual control over workflow execution, enabling testing, debugging, and demonstration without requiring chat triggers. This node allows developers to run the workflow with predefined inputs.

**Key Features:**
- Manual workflow triggering capability
- Configurable test parameters
- Useful for development and QA processes
- Bypass chat trigger for direct execution

**Screenshot Reference:** See `screenshots/02_workflow_config.png` for the manual configuration interface and trigger options.

---

### 3. Fetch NSE Stock Data (API Integration Node)

**Role:** Integrates with the National Stock Exchange (NSE) API to retrieve real-time financial data for the specified equity. This node fetches comprehensive market data including price, volume, financial ratios, and company fundamentals.

**Key Features:**
- Live NSE API connectivity
- Retrieves current market price, 52-week high/low
- Fetches fundamental data (P/E ratio, P/B ratio, market cap, debt levels)
- Error handling for API failures or invalid symbols
- Data validation and formatting

**Screenshot Reference:** See `screenshots/03_nse_api_node.png` for the API configuration, endpoint setup, and sample retrieved data.

---

### 4. Stock Analysis Agent (Custom AI Logic Node)

**Role:** Acts as the analytical engine of the workflow. This custom AI agent processes raw stock data and applies value investing principles to calculate key metrics such as margin of safety, intrinsic value, debt-to-equity ratios, and investment scores.

**Key Features:**
- Implements value investing calculations
- Computes margin of safety based on intrinsic value
- Analyzes financial health indicators
- Applies Benjamin Graham's investment criteria
- Generates quantitative scores for investment decisions
- Structures data for summarization

**Screenshot Reference:** See `screenshots/04_analysis_agent.png` for the custom logic implementation, calculation flows, and data processing steps.

---

### 5. OpenAI GPT-4 Turbo (AI Summarizer Node)

**Role:** Synthesizes all analytical findings into clear, actionable investment insights. This node leverages GPT-4 Turbo to translate complex financial data and metrics into easy-to-understand recommendations suitable for both novice and experienced investors.

**Key Features:**
- Natural language summary generation
- Converts technical metrics into plain English
- Provides investment recommendations with reasoning
- Highlights risks and opportunities
- Token-optimized prompt engineering
- Returns structured, readable output

**Screenshot Reference:** See `screenshots/05_gpt4_summarizer.png` for the AI model configuration, completion logs, and sample output formatting.

---

### 6. Memory/Tool/Output Parser (Supporting Nodes)

**Role:** Provides essential supporting functionality for the workflow, including state management, data transformation, formatting utilities, and output handling. These nodes ensure smooth data flow between major processing stages.

**Key Features:**
- Workflow state persistence
- Data format conversion and validation
- Output formatting and structuring
- Error handling and logging
- Context management for multi-step processes

**Screenshot Reference:** See `screenshots/06_supporting_nodes.png` for the supporting node configurations and data flow connections.

---

## Complete Workflow Visualization

For a comprehensive view of how all nodes connect and interact within the workflow, refer to:
- `screenshots/00_complete_workflow.png` - Full workflow architecture
- `screenshots/workflow_execution.png` - Live execution example with data flow

---

## Node Summary Table

| Node Name                    | Function                                                           | Screenshot Reference          |
|------------------------------|--------------------------------------------------------------------|------------------------------ |
| When Chat Message Received   | Triggers workflow on user input                                    | 01_trigger_node.png           |
| Workflow Configuration       | Allows manual/test workflow trigger                                | 02_workflow_config.png        |
| Fetch NSE Stock Data         | Fetches live stock data from NSE API                               | 03_nse_api_node.png           |
| Stock Analysis Agent         | Applies investment scoring and value metrics                       | 04_analysis_agent.png         |
| OpenAI GPT-4 Turbo           | Summarizes results in clear, readable language                     | 05_gpt4_summarizer.png        |
| Memory/Tool/Output Parser    | Supports data flow, formatting, and output handling                | 06_supporting_nodes.png       |

---

## Additional Resources

For more information about the workflow implementation:
- See `README.md` for project overview and setup instructions
- See `screenshots/README.md` for detailed screenshot descriptions and workflow stage documentation
