# VARIABILI — N8N_VALUTAZIONE_NUOVI_DISEGNI

## EMAIL
- PROVIDER: Gmail (test) → Aruba (produzione)
- TRIGGER: IMAP polling

## AI
- PROVIDER: Groq API
- MODELLO: da definire (llama3 vision o equivalente con supporto immagini)

## FILESYSTEM
- PERCORSO HOST: C:/Users/boron/Desktop/VALUTAZIONE NUOVI DISEGNI/
- PERCORSO DOCKER: /data/valutazione/

## GITHUB
- REPO: N8N_VALUTAZIONE_NUOVI_DISEGNI
- TABELLE: /TABELLE/TABELLA_MACCHINE.xlsx e TABELLA_MATERIALI.xlsx
- PROMPT: /PROMPT/PROMPT_PREVENTIVISTA.md

## N8N
- URL: https://n8n.paoloboronimo.it
- CONTAINER: n8n_app
- PORTA: 5678
