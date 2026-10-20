# Lab 19 – Proof of work

Project: News Summarizer (OpenAI + Cohere with retries, fallback and cost tracking).
Repository: https://github.com/jaimegmarquerie-ui/news-summarizer

## 1. Workflow / configuration
Files: `config.py`, `news_api.py`, `llm_providers.py`, `summarizer.py`, `main.py`, `test_summarizer.py`, `.env.example`, `.gitignore`, `requirements.txt`, `README.md`.

Settings used: `MAX_RETRIES=3`, `REQUEST_TIMEOUT=30`, `DAILY_BUDGET=5.00`, models `gpt-4o-mini` (OpenAI) and `command-r-08-2024` (Cohere).

Flow: NewsAPI → remove duplicates → summary (OpenAI, fallback Cohere) → sentiment (Cohere, fallback OpenAI) → cost report.

## 2. Execution trace (fallback)
Command: `python llm_providers.py fallback`

```
<PEGA AQUÍ LA SALIDA DEL COMANDO>
```

What this shows (in your own words): <ESCRIBE 1-2 FRASES>

## 3. Input payload (one article from NewsAPI)
```json
<PEGA AQUÍ EL ARTÍCULO>
```

## 4. Output record (same article, processed)
Command: `python summarizer.py 1`

```
<PEGA AQUÍ LA SALIDA>
```

What this shows (in your own words): <ESCRIBE 1-2 FRASES>

## 5. Tests
Command: `pytest test_summarizer.py -v` → **14 passed**. (Screenshot attached in the submission.)
