# NbS Toolkit Backend (Narmada Basin)

FastAPI backend with a bundled read-only SQLite database (`data/narmada_nbs_canonical.db`).

## Run locally

    python -m venv .venv
    .venv\Scripts\activate
    pip install -r requirements.txt
    python -m uvicorn app.main:app --reload --port 8000

Open http://127.0.0.1:8000/docs

## Deploy on Render

Render > New > Blueprint > pick this repo > Apply. Settings come from `render.yaml`.
After the frontend is live, set `CORS_ALLOW_ORIGINS` to the Netlify URL.
