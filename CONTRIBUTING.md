# Guida alla Contribuzione e Gestione Segnalazioni 📋

Benvenuto/a nell'ecosistema digitale di **Rovi Spazio Creativo ETS**. Per mantenere il nostro flusso di lavoro organizzato, essenziale e garantire interventi rapidi, utilizziamo un sistema centralizzato.

## 📝 1. Per chi Segnala (Come aprire una Issue)

Non è necessario sapere esattamente in quale modulo o repository si trovi il codice. Segui questi passaggi:

1. Clicca su **New Issue** in alto a destra.
2. Seleziona il template più adatto:
   - 🐛 **Segnalazione Bug**: Per errori, crash o comportamenti inattesi della piattaforma.
   - 💡 **Proposta Nuova Funzionalità**: Per suggerire idee, miglioramenti o espansioni.
3. **Compila il modulo** in ogni sua parte. Più contesto e dettagli fornisci (inclusi i passaggi per riprodurre un errore), più veloce sarà l'analisi.

---

## 🔀 2. Per il Team di Sviluppo (Processo di Triage)

Le nuove Issue vengono create automaticamente con la label `status: triage`. Chi fa da revisore (maintainer) segue questi step:

1. **Analisi e Assegnazione Area**
   Analizzare la richiesta e determinare i microservizi coinvolti. Rimuovere la label `status: triage` e applicare le label di competenza (che ti raccomandiamo di creare):
   - `area: frontend` / `area: UI`
   - `area: iam` (Autenticazione/Utenti)
   - `area: payments` (Transazioni/Gateway)
   - `area: core-api`
2. **Priorità e Stato**
   Assegnare una label di priorità (`P1: Critical`, `P2: High`, `P3: Medium`) e aggiornare lo stato (es. `status: in-progress`, `status: blocked`).
3. **Assegnazione**
   Assegnare (`Assignees`) la issue allo sviluppatore o al team incaricato.
4. **Trasferimento (Opzionale ma raccomandato)**
   Se si capisce che la issue riguarda in modo isolato un unico microservizio (es. un bug esclusivo del gateway di pagamento), è possibile cliccare su **Transfer issue** (nella barra laterale destra di GitHub) per spostarla direttamente nel repository `rovi-be-payments-service`.

## 📦 3. Promemoria Architettura
Per un triage rapido, tieni a mente la divisione dei nostri moduli:
- **`coworking_app`**: Esperienza utente, front-end e logica di orchestrazione (prenotazioni, spazi).
- **`rovi-gale1-iam-platform`**: Login, token di sicurezza, permessi utente.
- **`rovi-be-payments-service`**: Microservizio indipendente che processa denaro e abbonamenti (Stripe/PayPal, etc.).

Grazie per l'aiuto nel mantenere solida e affidabile l'infrastruttura di Rovi! 🌿
