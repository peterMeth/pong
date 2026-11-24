# Pong als App (PWA) über GitHub Pages

## Auf dem Handy installieren

1. Die Adresse in **Chrome** öffnen.
2. Im Menü (⋮) auf **App installieren** bzw. **Installieren und Verknüpfung erstellen ...** tippen.
3. Pong erscheint im App-Drawer, startet im Vollbild und läuft auch offline.

## Updates

Nach einer Änderung an den Dateien in `sw.js` die Zeile `const CACHE = 'pong-v1'` hochzählen (z. B. `pong-v2`) und neu hochladen. Die installierte App holt sich das Update beim nächsten Start mit Internet, sichtbar meist nach dem zweiten Start.
