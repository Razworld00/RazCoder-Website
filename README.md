# RazCode LLM Web

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
