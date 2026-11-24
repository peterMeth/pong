# Pong als App (PWA) über GitHub Pages

## Veröffentlichen (einmalig)

1. Auf github.com anmelden und oben rechts auf **+ → New repository** klicken.
2. Als Namen `pong` eingeben und **Public** wählen, dann auf **Create repository** klicken.
3. Auf der leeren Repo-Seite auf **uploading an existing file** klicken und den **Inhalt** dieses Ordners hineinziehen: `index.html`, `manifest.json`, `sw.js`, `README.md` und den Ordner `icons`. Danach **Commit changes** klicken.
4. **Settings → Pages** öffnen und unter *Build and deployment* Folgendes einstellen: Source **Deploy from a branch**, Branch **main**, Ordner **/ (root)**. Dann **Save** klicken.
5. Nach ca. 1 Minute ist das Spiel erreichbar unter
   `https://<dein-github-name>.github.io/pong/`

Alternativ per git:

```
git init
git add .
git commit -m "Pong PWA"
git branch -M main
git remote add origin https://github.com/<dein-github-name>/pong.git
git push -u origin main
```

Danach Schritt 4 wie oben.

## Auf dem Handy installieren

1. Die Adresse in **Chrome** öffnen.
2. Im Menü (⋮) auf **App installieren** (oder **Zum Startbildschirm hinzufügen → Installieren**) tippen.
3. Pong erscheint im App-Drawer, startet im Vollbild und läuft auch offline.

## Updates

Nach einer Änderung an den Dateien in `sw.js` die Zeile `const CACHE = 'pong-v1'` hochzählen (z. B. `pong-v2`) und neu hochladen. Die installierte App holt sich das Update beim nächsten Start mit Internet, sichtbar meist nach dem zweiten Start.
