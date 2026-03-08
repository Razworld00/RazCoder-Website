# RazCode LLM Web
# RazCoder

<p align="center">
  <img src="assets/razcoder-logo.svg" alt="RazCoder Logo" width="820" />
</p>

<p align="center">
  <strong>RazCoder Web</strong> Full-stack web interface for RazCode with modern LLM UX patterns
</p>

<p align="center">
  <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-green.svg"></a>
  <a href=".github/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/badge/CI-GitHub_Actions-blue.svg"></a>
  <img alt="Python" src="https://img.shields.io/badge/Python-3.10%2B-blue">
</p>


Full-stack web interface for RazCode with modern LLM UX patterns:

- Multi-session chat sidebar
- Provider/model switcher
- Markdown + code block rendering with copy buttons
- Live tool trace panel
- API backend powered by `RazCodeAgent`

## Run

```bash
cd /home/raz/RazCode/apps/razcode_llm_web
python app.py
```

Open:

- http://127.0.0.1:8099

## Environment

Optional:

- `PORT=8099`
- `HOST=127.0.0.1`
- `RAZCODE_WORKSPACE=/home/raz/RazCode`
- `RAZCODE_LLM_PROVIDER=ollama|openai|openrouter|groq|together|deepseek|fireworks`
- `RAZCODE_MODEL=...`

## API Endpoints

- `GET /api/health`
- `GET /api/providers`
- `GET /api/models?provider=<name>`
- `GET /api/sessions`
- `GET /api/sessions/<id>`
- `POST /api/sessions`
- `POST /api/chat`
