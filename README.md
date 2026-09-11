# 34-ImportExportSpecialist

Génère un rapport de conformité pour l'expédition d'un produit du Royaume-Uni vers le Maroc. Un agent répond aux exigences d'export UK / import marocain (licences, droits, TVA, articles interdits) à partir d'une base de connaissances construite depuis des PDF de droit commercial OCRisés (+ recherche DuckDuckGo en repli) ; un second agent recherche les réglementations locales de mise sur le marché. Les deux sorties sont combinées et converties en document Word téléchargeable.

## Tech stack

agno (Agent, Groq, Knowledge/LanceDb, MistralEmbedder, DuckDuckGoTools), mistralai (OCR), markdown2, html2docx, python-dotenv

## Lancer le projet

```bash
pip install agno mistralai markdown2 html2docx python-dotenv
```

Créer un `.env` avec `GROQ_API_KEY=...` et `MISTRAL_API_KEY=...`

```bash
python full_import_export_agent.py
```
