# Node Descriptions

## Node List and Descriptions:

### 1. When Chat Message Received (Trigger Node)

**Role:** Listens for user input to start the analysis workflow.

**Screenshot suggestion:** Show the chat window and trigger configuration.

### 2. Workflow Configuration (Manual Node)

**Role:** Allows you to manually trigger the workflow for testing or demonstration purposes.

**Screenshot suggestion:** Show configuration and manual trigger option.

### 3. Fetch NSE Stock Data (API Integration Node)

**Role:** Connects to the National Stock Exchange API, fetches the latest financial data for the target equity.

**Screenshot suggestion:** Show node setup with API details and retrieved data example.

### 4. Stock Analysis Agent (Custom AI Logic Node)

**Role:** Processes stock data, applies value-investing calculations (margin of safety, P/E, P/B, debt ratios), and organizes for further analysis.

**Screenshot suggestion:** Display node internal logic setup and data flow.

### 5. OpenAI GPT-4 Turbo (AI Summarizer Node)

**Role:** Summarizes all findings and presents analysis in readable, non-technical language. Handles token usage and returns clear output.

**Screenshot suggestion:** Show completion logs, output, and success status.

### 6. Memory/Tool/Output Parser (Supporting Nodes)

**Role:** Provide state management, auxiliary functions (e.g., formatting data), and handle workflow output.

---

## Sample Markdown Table for Node Documentation:

| Node Name                    | Function                                                           |
|------------------------------|--------------------------------------------------------------------||
| When Chat Message Received   | Triggers workflow on user input                                    |
| Workflow Configuration       | Allows manual/test workflow trigger                                |
| Fetch NSE Stock Data         | Fetches live stock data from NSE                                   |
| Stock Analysis Agent         | Applies investment scoring, value metrics                          |
| OpenAI GPT-4 Turbo           | Summarizes results in clear, readable language                     |
| Memory/Tool/Output Parser    | Supports data flow, formatting, and output                         |
