# Screenshots Documentation

This directory contains visual documentation of the Indian Equity Investment Stock Analyzer workflow. Each screenshot captures a specific node configuration or workflow stage, providing visual reference for implementation and understanding.

---

## Complete Workflow Overview

### 00_complete_workflow.jpg
**Description:** Full end-to-end workflow architecture diagram showing all nodes and their connections.

**Details:**
- Displays the complete data flow from trigger to final output
- Shows how all 6 major nodes interconnect
- Visualizes the sequence: Chat Trigger → Configuration → NSE API → Analysis Agent → GPT-4 Summarizer → Output
- Useful for understanding the overall system architecture

**Workflow Stage:** Complete System Overview

---

## Node-Specific Screenshots

### 01_trigger_node.jpg
**Node:** When Chat Message Received (Trigger Node)

**Description:** Configuration and setup of the chat message trigger that initiates the workflow.

**Details:**
- Shows trigger configuration parameters
- Displays message parsing logic for extracting stock symbols
- Demonstrates how user input is captured and forwarded
- Includes webhook or event listener setup

**Workflow Stage:** Entry Point / User Input

---

### 02_workflow_config.jpg
**Node:** Workflow Configuration (Manual Node)

**Description:** Manual workflow trigger and configuration interface.

**Details:**
- Displays manual execution controls
- Shows test input fields for stock symbols
- Demonstrates debugging and development mode options
- Includes parameter configuration for workflow testing

**Workflow Stage:** Development & Testing

---

### 03_nse_api_node.jpg
**Node:** Fetch NSE Stock Data (API Integration Node)

**Description:** NSE API integration setup and live data retrieval demonstration.

**Details:**
- Shows NSE India API endpoint configuration
- Displays real-time stock data fetch parameters
- Demonstrates data extraction and parsing logic
- Includes error handling and fallback mechanisms
- Shows sample response data structure

**Workflow Stage:** Data Acquisition

---

### 04_analysis_agent.jpg
**Node:** Stock Value Analysis Agent (Core Analysis Engine)

**Description:** Value investing analysis agent configuration and calculation logic.

**Details:**
- Shows Benjamin Graham's value investing formula implementation
- Displays P/E ratio, EPS, and book value calculations
- Demonstrates fair value computation logic
- Shows safety margin calculation (current price vs. fair value)
- Includes data validation and error handling
- Demonstrates recommendation engine logic (Strong Buy, Buy, Hold, Sell)

**Workflow Stage:** Analysis & Calculation

---

### 05_gpt4_summarizer.jpg
**Node:** GPT-4 Turbo Summarizer (Natural Language Output)

**Description:** GPT-4 Turbo integration for generating natural language investment summaries.

**Details:**
- Shows OpenAI API configuration
- Displays prompt engineering for financial analysis
- Demonstrates structured data to narrative conversion
- Shows model parameters (temperature, tokens, etc.)
- Includes sample output formatting

**Workflow Stage:** Natural Language Generation

---

### 06_supporting_nodes.jpg
**Node:** Supporting Infrastructure Nodes

**Description:** Various supporting nodes that handle memory, parsing, and output processing.

**Details:**
- Chat Memory Node: Maintains conversation context
- Message Parsing Nodes: Extract stock symbols from user input
- Output Formatting Nodes: Structure final response
- Error Handling Nodes: Manage failures gracefully
- Logging and Debugging Nodes: Track workflow execution

**Workflow Stage:** Infrastructure & Support

---

### workflow_execution.jpg
**Description:** Complete workflow execution demonstration with live data.

**Details:**
- Shows actual workflow run with real stock data
- Displays data flow through all nodes
- Demonstrates successful execution from trigger to output
- Shows final formatted response
- Includes execution timing and performance metrics

**Workflow Stage:** Complete Execution Demo

---

## Screenshots Quick Reference

| Screenshot File               | Node/Component                        | Description                                       |
|-------------------------------|---------------------------------------|---------------------------------------------------|
| 00_complete_workflow.jpg      | Full Workflow                         | Complete workflow architecture diagram            |
| 01_trigger_node.jpg           | Chat Message Trigger                  | Entry point configuration                         |
| 02_workflow_config.jpg        | Manual Configuration                  | Testing and development setup                     |
| 03_nse_api_node.jpg           | NSE API Integration                   | Live data retrieval configuration                 |
| 04_analysis_agent.jpg         | Stock Analysis Agent                  | Value investing calculations and logic            |
| 05_gpt4_summarizer.jpg        | GPT-4 Turbo Summarizer                | AI-powered natural language output                |
| 06_supporting_nodes.jpg       | Supporting Infrastructure             | Memory, parsing, and output handling              |
| workflow_execution.jpg        | Complete Execution                    | Live demonstration of full workflow               |

---

## Using These Screenshots

### For Implementation
- Reference screenshots when configuring each node
- Use as a visual guide for parameter settings
- Compare your setup with the documented configurations

### For Troubleshooting
- Compare actual vs. expected node configurations
- Verify data flow matches the documented architecture
- Check API responses against sample data shown

### For Documentation
- Include in presentations and technical documentation
- Use for onboarding new developers
- Reference in README and setup guides

---

## Related Documentation

For detailed textual descriptions of each node:
- See `../nodes.md` for comprehensive node descriptions
- See `../README.md` for project overview and setup instructions

---

## Notes

- All screenshots are taken from the n8n workflow automation platform
- Screenshots show actual production configuration
- Sensitive information (API keys, credentials) has been redacted where necessary
- Screenshots are current as of the latest workflow version

---

**Last Updated:** October 2025  
**Workflow Version:** Latest  
**Platform:** n8n
