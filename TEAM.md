# Team di Sviluppo — Rovi Spazio Creativo ETS 🌿

Composizione del team dev, aree di competenza e flussi di revisione.
Gli username GitHub verranno aggiunti in CODEOWNERS una volta definiti.

## Ruoli e competenze

| Persona | Competenze | Aree / label |
|---|---|---|
| **Luca Rosati** | Presidente · gestione org e repository · richieste feature e UI/UX · product | product, `area: UI` |
| **Daniele Ciucci** | Architettura · flussi pagamenti · sicurezza applicativa · frontend | `area: payments`, `area: frontend`, security |
| **Gianmarco Innocenzi** | Codice backend · API e chiamate | `area: core-api` |
| **Andrea Ceccarelli** | Configurazione · Docker Compose · dimensionamento macchine · Oracle Cloud · IAM | `area: infra`, `area: iam` |
| **Francesco Battisti** | Dominio dell'applicazione · SEO e indicizzazione | `area: seo-domain` |

## Struttura del team

```mermaid
graph TD
    LR["Luca Rosati<br/>Presidente — Product / UX<br/>Gestione org e repository"]
    DC["Daniele Ciucci<br/>Architettura — Payments<br/>Security — Frontend"]
    GI["Gianmarco Innocenzi<br/>Backend — Core API"]
    AC["Andrea Ceccarelli<br/>Infra — Oracle Cloud<br/>IAM — Config / Compose"]
    FB["Francesco Battisti<br/>Dominio applicazione<br/>SEO e indicizzazione"]

    LR --> DC
    LR --> GI
    LR --> AC
    LR --> FB
```

## Flusso di revisione (secondo revisore)

Ogni area ha un owner primario e un secondo revisore di backup,
per evitare colli di bottiglia e single point of failure.

```mermaid
graph LR
    DC["Daniele Ciucci"]
    GI["Gianmarco Innocenzi"]
    AC["Andrea Ceccarelli"]

    DC -->|rivede le PR di| GI
    DC -->|rivede le PR di| AC
    AC -->|rivede le PR di| DC
```

- **Daniele ↔ Andrea**: si rivedono a vicenda (payments/frontend/security ↔ infra/iam).
- **Gianmarco** (core-api): rivisto da **Daniele**.

## Mappa area → owner → secondo revisore

| Label | Owner primario | Secondo revisore |
|---|---|---|
| `area: payments` | Daniele Ciucci | Andrea Ceccarelli |
| `area: frontend` | Daniele Ciucci | Andrea Ceccarelli |
| `area: core-api` | Gianmarco Innocenzi | Daniele Ciucci |
| `area: iam` | Andrea Ceccarelli | Daniele Ciucci |
| `area: infra` | Andrea Ceccarelli | Daniele Ciucci |
| `area: seo-domain` | Francesco Battisti | — |
