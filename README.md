# .github — Default community files di Rovi Spazio Creativo ETS

Questo repository contiene i file che fanno da **default per tutta l'organizzazione** `rovi-spazio` su GitHub: template di issue e PR, workflow di automazione, policy e documentazione del team.

## 📚 Indice

- [`profile/README.md`](./profile/README.md) — pagina pubblica dell'organizzazione
- [`CONTRIBUTING.md`](./CONTRIBUTING.md) — guida alla contribuzione e processo di triage
- [`SECURITY.md`](./SECURITY.md) — policy di sicurezza e segnalazione vulnerabilità
- [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) — codice di condotta
- [`TEAM.md`](./TEAM.md) — composizione del team `rovi-dev-lab` e flussi di revisione
- [`.github/ISSUE_TEMPLATE/`](./.github/ISSUE_TEMPLATE/) — template bug report e feature request
- [`.github/workflows/`](./.github/workflows/) — automazioni GitHub Actions

## 🤖 Automazioni attive

- **welcome.yml** — saluto automatico alla prima issue/PR di un contributor
- **stale.yml** — chiusura automatica di issue/PR inattive da oltre 60 giorni
- **triage-labeler.yml** — applica automaticamente le label `area:` ai bug report leggendo i campi del modulo

## 👥 Team

Il team di sviluppo è organizzato sotto il team genitore `@rovi-spazio/rovi-dev-lab`, con sotto-team per area di competenza. Vedi [TEAM.md](./TEAM.md) per la composizione completa.