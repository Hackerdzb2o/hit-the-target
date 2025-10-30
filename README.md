# Hit the Target Game

Piccolo sito statico con il gioco *Hit the Target* (desktop only).

## Contenuto
- `index.html` — pagina principale (gioco desktop, clic con mouse).
- `.github/workflows/gh-pages.yml` — workflow opzionale per deploy su GitHub Pages (branch `gh-pages`).
- Non ci sono suoni, né salvataggio del punteggio: tutto è volutamente minimale.

## Pubblicazione su GitHub Pages (metodo semplice)
1. Crea un nuovo repository su GitHub (es. `hit-the-target`).
2. Estrai i file di questo pacchetto e carica tutto il contenuto nella root del repository.
   - Puoi usare l'interfaccia web ("Upload files") oppure `git` da terminale.
3. Sul repository GitHub vai in **Settings → Pages**.
   - Seleziona la branch `gh-pages` (se hai usato il workflow), oppure `main` (se hai caricato i file direttamente).
   - Salva. Dopo alcuni secondi/minuti il sito sarà disponibile all'URL:
     `https://TUOUSERNAME.github.io/NOME-REPO/`

## Comandi rapidi con `git`
```bash
git init
git add .
git commit -m "Initial commit - hit the target"
git branch -M main
git remote add origin git@github.com:TUOUSERNAME/hit-the-target.git
git push -u origin main
```

Se preferisci usare il workflow GitHub Actions (automazione al push), il file `.github/workflows/gh-pages.yml` incluso esegue il deploy sulla branch `gh-pages`. In tal caso:
1. Crea il repository e spingi la branch `main` come sopra.
2. Modifica il workflow se necessario (il file è pronto per l'uso).
3. Abilita GitHub Pages per servire la branch `gh-pages` (Settings → Pages → branch `gh-pages`).

---

Se vuoi, ti posso:
- spiegare passo-passo come creare il repository e caricare i file (con screenshot testuali), oppure
- generare i comandi `git` personalizzati con il tuo nome utente GitHub (se me lo dai).
