# taubenundco-support

Öffentliche Hilfe- und Datenschutzseite zur App **Tauben & Co**
(`de.taubenundco.app`, iPhone und Android).

Google Play verlangt eine öffentlich erreichbare Datenschutz-URL, App Store
Connect zusätzlich eine Support-URL. Die eigentliche Webseite der Vogelstation
(taubenundco.de) liegt hinter einem Anmelde-Tor und kommt dafür nicht in Frage —
deshalb diese Seite über GitHub Pages.

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: was die App ist, Support-Kontakt |
| `datenschutz.html` | Datenschutzerklärung (Play: Datenschutz-URL) |
| `.nojekyll` | GitHub Pages soll die Dateien unverändert ausliefern |

Die Quelle von `datenschutz.html` liegt im App-Projekt unter
`app/server/srv/avian/oeffentlich/app/datenschutz.html`. Änderungen gehören
dorthin und werden von hier aus nur kopiert.

Kein Skript, keine fremden Schriften, kein externer Aufruf. Keine Daten aus der
Station: keine Aufnahmen, keine Fundzahlen, keine Standortadressen.
