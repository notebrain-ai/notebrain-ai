# AI Setup

NoteBrain includes a built-in AI assistant that can answer questions using your notes as context. There are three ways to use it:

## Option 1: Own API keys (free, unlimited)

Bring your own API key from any supported provider. No subscription needed.

1. Open **Settings** > **AI**
2. Select your provider: Gemini, OpenAI, or Claude
3. Paste your API key
4. Start chatting

Supported providers:

| Provider | Models | Get a key |
|----------|--------|-----------|
| Google Gemini | Gemini Flash, Gemini Pro | [ai.google.dev](https://ai.google.dev) |
| OpenAI | GPT-4o, GPT-4o-mini | [platform.openai.com](https://platform.openai.com) |
| Anthropic Claude | Claude Sonnet, Claude Haiku | [console.anthropic.com](https://console.anthropic.com) |

## Option 2: Ollama (free, local, desktop only)

Run AI completely on your machine with no internet connection needed.

1. Install [Ollama](https://ollama.ai)
2. Pull a model: `ollama pull llama3.2`
3. Open **Settings** > **AI** > select **Ollama**
4. NoteBrain will detect it automatically

## Option 3: NoteBrain Cloud AI (subscription)

No API keys to manage. Just sign in and chat.

- **Free tier** — 100K tokens included
- **AI Starter** (3 EUR/mo) — 1M tokens/month
- **AI Pro** (6 EUR/mo) — 5M tokens/month + Gemini Pro model

## How RAG works

When you ask a question, NoteBrain:

1. Searches your notes for relevant content (full-text search)
2. Sends the question + relevant context to the AI
3. The AI answers based on your actual notes

Your notes are never stored on external servers when using own API keys or Ollama. With cloud AI, context is sent to Google's Vertex AI for processing but not retained.
