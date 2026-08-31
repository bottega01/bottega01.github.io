# bottega01.github.io

Sito pubblico di bottega01 — www.bottega01.com

Pagina statica, nessun build, nessuna dipendenza esterna a runtime.

## Cosa modificare, e dove

Tutto sta dentro `index.html`, in cima al blocco `<script>`.

- **`SITE.email`** — indirizzo di contatto mostrato nella sezione Contatti.
- **`APP_CATALOG`** — una voce per app. Per aggiungerne una: `name`, `appId`,
  `store`, `icon`, e i testi `it` / `en`. La numerazione e' automatica.
- **`COPY.it` / `COPY.en`** — tutti i testi delle due lingue, uno sotto l'altro.

## Icone

Stanno in `icons/`, servite da questo repo. Vedi `icons/LEGGIMI.txt` per i nomi
dei file. Nessuna chiamata ad Apple a runtime: le icone non spariscono se Apple
limita le richieste, e l'IP dei visitatori non esce da qui.

## Font

IBM Plex Sans e IBM Plex Mono, SIL Open Font License 1.1, in `fonts/`.
Sottoinsiemi latin e latin-ext, pesi 400/500/600. Serviti dal repo, non da
Google: nessun dato dei visitatori inviato a terzi, quindi nessun cartello
cookie da mettere.

## Pubblicazione

GitHub Pages, radice del repository, branch principale. Nessun comando di build.
Il file `.nojekyll` disattiva l'elaborazione Jekyll: non toccarlo.
Il dominio custom si imposta da Settings > Pages, non creando il file CNAME a mano.
