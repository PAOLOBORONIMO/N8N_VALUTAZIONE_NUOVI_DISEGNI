# NOTE — N8N_VALUTAZIONE_NUOVI_DISEGNI

## ARCHITETTURA WORKFLOW
1. Gmail IMAP -> classificazione mail (ORDINE / OFFERTA / SPAM / APPROVVIGIONAMENTO / INFO)
2. Se ORDINE o OFFERTA con allegati -> crea cartella cliente in /data/valutazione/[CLIENTE]/
3. Scarica allegati (PDF / immagini disegni tecnici)
4. Groq AI analizza ogni disegno con PROMPT_PREVENTIVISTA
5. Annota il file originale con ciclo di lavoro estratto
6. Salva file annotato nella cartella cliente

## NOTE TECNICHE
- Saldatura: ESTERNALIZZATA (no macchine interne)
- Trattamenti: ESTERNALIZZATI
- Laser lamiera: campo max 1500x3000mm -> sviluppo superiore = esternalizzare
- Piegatrice: campo max 3000mm -> sviluppo superiore = esternalizzare
- Tubolari/Tubi/Barre: gestione a commessa, L.commerciale 6000mm

## PROSSIMI PASSI
- [ ] Costruire workflow n8n completo
- [ ] Configurare credenziali Gmail in n8n
- [ ] Configurare API Groq in n8n
- [ ] Testare con disegno campione
- [ ] Implementare annotazione PDF
