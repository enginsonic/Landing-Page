# VisualSync — sito

Landing page di **VisualSync**, app macOS nativa che mette una giacca e cravatta
a `rsync`: un front-end visuale per backup e mirroring di cartelle, con profili
salvati, anteprima a vuoto prima di ogni sync e una vista a due pannelli.

Sito statico: `index.html` + `landing.css` + `assets/`. Nessun build, nessun backend.

---

## Cos'è rsync (e perché VisualSync gli deve tutto)

[`rsync`](https://rsync.samba.org/) è l'utility da riga di comando che dal 1996 è
lo standard de facto per **sincronizzare e copiare file** in modo efficiente: invia
solo le differenze tra sorgente e destinazione (delta-transfer), preserva permessi
e metadati, gestisce link e cancellazioni, e gira su praticamente qualunque sistema
Unix. È il motore che fa il lavoro vero — VisualSync è solo la carrozzeria.

- 🌐 Sito ufficiale: <https://rsync.samba.org/>
- 📦 Repository originale: <https://github.com/RsyncProject/rsync>
- 👤 Creato da **Andrew Tridgell** e **Paul Mackerras**, oggi mantenuto da
  **Wayne Davison** e dalla comunità. Licenza GPLv3.

## Riconoscenza

VisualSync esiste solo perché altri hanno fatto il lavoro difficile. Un grazie a:

- **Andrew Tridgell** — per rsync (e Samba): il lavoro di riferimento su cui
  poggia tutto questo progetto.
- I **mantenitori e contributori di rsync** — per trent'anni di affidabilità.
- Il progetto [**openrsync**](https://github.com/kristapsdz/openrsync) — la
  reimplementazione BSD-licenziata, oggi inclusa anche in macOS.

E agli altri front-end e strumenti di sync che hanno tracciato la strada, da cui
abbiamo imparato e a cui va il nostro rispetto:

- [**Grsync**](http://www.opbyte.it/grsync/) — storica GUI GTK per rsync su Linux.
- [**rsnapshot**](https://rsnapshot.org/) — snapshot di filesystem costruiti su rsync.
- [**Unison**](https://www.cis.upenn.edu/~bcpierce/unison/) — sincronizzazione
  bidirezionale.
- [**FreeFileSync**](https://freefilesync.org/) — confronto e sync di cartelle
  multipiattaforma.
- **Carbon Copy Cloner** e **ChronoSync** — i riferimenti commerciali del backup su macOS.

VisualSync non vuole sostituire nessuno di questi: vuole solo rendere rsync
ovvio per chi non vive nel terminale.

---

## Come si aggiorna il sito

1. Modifica i file in questa cartella (il design nasce in Claude Design, poi si copia qui).
2. In GitHub Desktop: scrivi un messaggio → **Commit** → **Push**.
3. GitHub Pages ripubblica da solo in ~30 secondi.

## Link da collegare quando pronti

- Pulsanti "Download .dmg" → URL della GitHub Release dell'app
  (`releases/latest/download/VisualSync.dmg`).
- Link "GitHub" → repo dell'app.
