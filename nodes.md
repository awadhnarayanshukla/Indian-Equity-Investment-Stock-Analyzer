# Node Reference

| Node | Purpose | Key Parameters | Notes |
|------|---------|----------------|-------|
| Trigger | Starts the workflow on demand | Input: ticker symbol | Use Manual Trigger for testing. |
| HTTP Request (NSE) | Fetch latest stock data | Method: GET; URL: NSE endpoint; Query: symbol | Ensure compliance with NSE terms; consider caching. |
| Code | Compute value indicators | Inputs: price, EPS, ROE, etc. | JavaScript in n8n Code node to derive metrics. |
| OpenAI (Chat) | Generate plain-English summary | Model: GPT-4/Turbo; Prompt template | Include computed metrics and disclaimers. |
| Set/Function | Normalize fields | Mapping of raw -> normalized keys | Keeps downstream nodes consistent. |
| Merge/IF | Control flow based on data quality | Conditions on null/thresholds | Route to fallback or error summary if needed. |
| Markdown/HTML | Produce readable output | Template with metrics table | For rendering in n8n execution. |

References
- n8n Docs: https://docs.n8n.io/
- HTTP Request: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httpRequest/
- Code Node: https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/
- OpenAI: https://docs.n8n.io/integrations/builtin/ai-openai/
