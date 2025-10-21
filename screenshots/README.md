# Screenshots Documentation

This directory contains visual documentation of the Indian Equity Investment Stock Analyzer workflow. Each screenshot captures a specific node configuration or workflow stage, providing visual reference for implementation and understanding.

---

## Complete Workflow Overview

### 00_complete_workflow.png
**Description:** Full end-to-end workflow architecture diagram showing all nodes and their connections.

**Details:**
- Displays the complete data flow from trigger to final output
- Shows how all 6 major nodes interconnect
- Visualizes the sequence: Chat Trigger → Configuration → NSE API → Analysis Agent → GPT-4 Summarizer → Output
- Useful for understanding the overall system architecture

**Workflow Stage:** Complete System Overview

---

## Node-Specific Screenshots

### 01_trigger_node.png
**Node:** When Chat Message Received (Trigger Node)

**Description:** Configuration and setup of the chat message trigger that initiates the workflow.

**Details:**
- Shows trigger configuration parameters
- Displays message parsing logic for extracting stock symbols
- Demonstrates how user input is captured and forwarded
- Includes webhook or event listener setup

**Workflow Stage:** Entry Point / User Input

---

### 02_workflow_config.png
**Node:** Workflow Configuration (Manual Node)

**Description:** Manual workflow trigger and configuration interface.

**Details:**
- Displays manual execution controls
- Shows test input fields for stock symbols
- Demonstrates debugging and development mode options
- Includes parameter configuration for workflow testing

**Workflow Stage:** Development & Testing

---

### 03_nse_api_node.png
**Node:** Fetch NSE Stock Data (API Integration Node)

**Description:** NSE API integration setup and live data retrieval demonstration.

**Details:**
- Shows API endpoint configuration
- Displays authentication and header setup
- Demonstrates sample API response with stock data
- Includes error handling configuration
- Shows data fields: current price, 52-week high/low, P/E ratio, P/B ratio, market cap, debt levels

**Workflow Stage:** Data Acquisition

---

### 04_analysis_agent.png
**Node:** Stock Analysis Agent (Custom AI Logic Node)

**Description:** Custom AI agent logic for value investing calculations and stock analysis.

**Details:**
- Shows implementation of value investing formulas
- Displays margin of safety calculations
- Demonstrates intrinsic value computation logic
- Shows debt-to-equity ratio analysis
- Includes Benjamin Graham's investment criteria implementation
- Visualizes data transformation and scoring algorithms

**Workflow Stage:** Analysis & Computation

---

### 05_gpt4_summarizer.png
**Node:** OpenAI GPT-4 Turbo (AI Summarizer Node)

**Description:** GPT-4 Turbo configuration for generating natural language investment summaries.

**Details:**
- Shows OpenAI API configuration
- Displays prompt engineering for investment analysis
- Demonstrates model parameters (temperature, max tokens, etc.)
- Includes sample AI-generated summary output
- Shows how technical metrics are translated to readable recommendations

**Workflow Stage:** Natural Language Generation / Final Output

---

### 06_supporting_nodes.png
**Node:** Memory/Tool/Output Parser (Supporting Nodes)

**Description:** Supporting infrastructure including memory management, data parsers, and output formatters.

**Details:**
- Shows memory/state management configuration
- Displays data transformation tools
- Demonstrates output formatting logic
- Includes error handling and logging setup
- Shows connections between major nodes

**Workflow Stage:** Data Flow Management

---

## Additional Workflow Documentation

### workflow_execution.png
**Description:** Live workflow execution example showing real-time data flow and processing.

**Details:**
- Captures a live run with actual stock data
- Shows data passing through each node
- Demonstrates successful execution from input to output
- Highlights execution timing and performance metrics
- Useful for troubleshooting and performance optimization

**Workflow Stage:** Live Execution Example

---

## Screenshot Organization

| Screenshot File               | Node/Component                        | Purpose                                          |
|-------------------------------|---------------------------------------|--------------------------------------------------|
| 00_complete_workflow.png      | Full Workflow                         | System architecture overview                     |
| 01_trigger_node.png           | Chat Message Trigger                  | Entry point configuration                        |
| 02_workflow_config.png        | Manual Configuration                  | Testing and development setup                    |
| 03_nse_api_node.png           | NSE API Integration                   | Live data retrieval configuration                |
| 04_analysis_agent.png         | Stock Analysis Agent                  | Value investing calculations and logic           |
| 05_gpt4_summarizer.png        | GPT-4 Turbo Summarizer                | AI-powered natural language output               |
| 06_supporting_nodes.png       | Supporting Infrastructure             | Memory, parsing, and output handling             |
| workflow_execution.png        | Complete Execution                    | Live demonstration of full workflow              |

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
