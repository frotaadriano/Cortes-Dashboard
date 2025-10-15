# 🎬 cortes-dashboard


A FastAPI + FFmpeg + yt-dlp dashboard to plan, preview, and automatically cut YouTube clips with AI-assisted tooling.


## Features
- Preview YouTube videos in the browser
- Mark In/Out timestamps with keyboard shortcuts
- One-click API calls to download, cut (manual or automatic by silence), normalize audio, and burn subtitles
- Consistent output in `outputs/` and temp files in `work/`


## Quickstart
```bash
python -m venv .venv && source .venv/bin/activate # Windows: .venv\Scripts\activate
pip install -r requirements.txt
# Install FFmpeg (see README body for OS-specific commands)
uvicorn backend.main:app --reload
# Open http://localhost:8000 (frontend served by FastAPI)
```


---


## 🇧🇷 Descrição
Dashboard com FastAPI, FFmpeg e yt-dlp para planejar, visualizar e cortar vídeos do YouTube automaticamente com ajuda de IA.


### Fluxo
1. Insira a URL do YouTube
2. Marque os trechos (In/Out) e adicione à lista
3. Clique nos botões de API para baixar, cortar, normalizar e queimar legendas


> Saídas finais em `outputs/`, originais e legendas em `work/`.


---


## Notes
- Ensure you have permission to reuse the source content.
- You may need to adjust FFmpeg parameters for specific videos (keyframe cutting vs re-encode).
