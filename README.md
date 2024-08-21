# ai_api_pricing

This repository summarizes pricing information for major AI API providers. We compare the prices of the following APIs:

- OpenAI API
- Anthropic API
- Google Gemini API

## OpenAI API Pricing

### GPT-4 Models

| Model | Input (per 1M tokens) | Output (per 1M tokens) | Input with Batch API* | Output with Batch API* |
|-------|------------------------|------------------------|------------------------|-------------------------|
| gpt-4o | $5.000 | $15.000 | $2.500 | $7.500 |
| gpt-4o-2024-08-06 | $2.500 | $10.000 | $1.875 | $7.500 |
| gpt-4o-2024-05-13 | $5.000 | $15.000 | $2.500 | $7.500 |
| gpt-4o-mini | $0.150 | $0.600 | $0.075 | $0.300 |
| gpt-4o-mini-2024-07-18 | $0.150 | $0.600 | $0.075 | $0.300 |

### Embedding Models

| Model | Price (per 1M tokens) | Price with Batch API* |
|-------|------------------------|------------------------|
| text-embedding-3-small | $0.020 | $0.010 |
| text-embedding-3-large | $0.130 | $0.065 |
| ada v2 | $0.100 | $0.050 |

### Fine-tuning Models

| Model | Input (per 1M tokens) | Output (per 1M tokens) | Input with Batch API* | Output with Batch API* | Training (per 1M tokens) |
|-------|------------------------|------------------------|------------------------|-------------------------|---------------------------|
| gpt-4o-2024-08-06** | $3.750 | $15.000 | $1.875 | $7.500 | $25.000 |
| gpt-4o-mini-2024-07-18** | $0.300 | $1.200 | $0.150 | $0.600 | $3.000 |
| gpt-3.5-turbo | $3.000 | $6.000 | $1.500 | $3.000 | $8.000 |
| davinci-002 | $12.000 | $12.000 | $6.000 | $6.000 | $6.000 |
| babbage-002 | $1.600 | $1.600 | $0.800 | $0.800 | $0.400 |

*Batch API pricing may be subject to specific conditions or availability.
**Fine-tuning for these models may have additional requirements or limitations.

## Anthropic API Pricing

| Model | Context Window | Input | Output | Prompt Caching Write | Prompt Caching Read |
|-------|----------------|-------|--------|----------------------|---------------------|
| Claude 3.5 Sonnet | 200K | $3 / MTok | $15 / MTok | $3.75 / MTok | $0.30 / MTok |
| Claude 3 Opus | 200K | $15 / MTok | $75 / MTok | $18.75 / MTok (Coming Soon) | $1.50 / MTok (Coming Soon) |
| Claude 3 Haiku | 200K | $0.25 / MTok | $1.25 / MTok | $0.30 / MTok | $0.03 / MTok |

Note: Prices are per million tokens (MTok).

## Google Gemini API Pricing

| Model | Feature | Type | Price (≤ 128K context window) | Price (> 128K context window) |
|-------|---------|------|-------------------------------|-------------------------------|
| Gemini 1.5 Flash | Multimodal | Image Input | $0.00002 / image | $0.00004 / image |
| | | Video Input | $0.00002 / second | $0.00004 / second |
| | | Text Input | $0.00001875 / 1k characters | $0.0000375 / 1k characters |
| | | Audio Input | $0.000002 / second | $0.000004 / second |
| | | Text Output | $0.000075 / 1k characters | $0.00015 / 1k characters |
| Gemini 1.5 Pro | Multimodal | Image Input | $0.001315 / image | $0.00263 / image |
| | | Video Input | $0.001315 / second | $0.00263 / second |
| | | Text Input | $0.00125 / 1k characters | $0.0025 / 1k characters |
| | | Audio Input | $0.000125 / second | $0.00025 / second |
| | | Text Output | $0.00375 / 1k characters | $0.0075 / 1k characters |
| Gemini 1.0 Pro | Multimodal | Image Input | $0.0025 / image | - |
| | | Video Input | $0.002 / second | - |
| | | Text Input | $0.000125 / 1k characters | - |
| | | Text Output | $0.000375 / 1k characters | - |
| Grounding with Google Search | Text | Grounding requests | $35 / 1k requests (for up to 1M requests per day) | - |

### Supplementary Information: 128K Context Window

The 128K context window refers to the maximum amount of text that an AI language model can process at once. Here's what it means in practical terms:

1. Size: It can process approximately 128,000 tokens (words or parts of words) at a time.

2. Character count: This translates to roughly 500,000 to 800,000 characters (varying by language and content).

3. Length examples:
   - Equivalent to 1-2 average books
   - Several long academic papers
   - Transcripts of multiple hours of conversation

4. Advantages:
   - Allows for understanding of longer contexts
   - Can process complex arguments or detailed explanations in one go
   - Enables summarization and analysis of lengthy documents

5. Limitations:
   - Text exceeding this amount needs to be split for processing
   - Still has constraints in fully comprehending very long documents in their entirety

The 128K context window represents a significant advancement in AI technology, enabling the handling of more complex and lengthy tasks.