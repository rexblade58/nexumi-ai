# Nexumi AI

Multi-model AI assistant platform with web client and API backend.

## Architecture

```
nexumi-ai/
  apps/web/        React frontend with TypeScript and Tailwind
  backend/         Express API server with proxy endpoints
```

## Quick Start

```bash
git clone https://github.com/rexblade58/nexumi-ai.git
cd nexumi-ai
npm install
npm run dev
```

## Features

- Chat interface with streaming responses
- Multi-model support via OpenRouter and Together AI
- Local model support through Ollama
- Image generation and analysis endpoints
- Offline detection with graceful fallback
- Web worker for background AI processing

## API

| Endpoint | Method | Description |
| :--- | :--- | :--- |
| `/health` | GET | Health check and uptime |
| `/api/chat` | POST | Chat completion proxy |
| `/api/generate-image` | POST | Image generation via FLUX.1 |
| `/api/analyze-image` | POST | Image analysis via Gemini |

## Tech Stack

| Layer | Technologies |
| :--- | :--- |
| Frontend | React 18, TypeScript, Vite, Tailwind CSS, Zustand |
| Backend | Node.js, Express, CORS, Axios |
| AI | OpenAI SDK, OpenRouter, Together AI, Ollama |

## Branch Strategy

| Branch | Purpose |
| :--- | :--- |
| `main` | Production releases |
| `develop` | Active development and integration |
| `staging` | Pre-release testing and QA |

## License

MIT (c) 2021-2025 Menard Rosal