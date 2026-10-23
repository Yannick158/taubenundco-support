# taubenundco-support

Öffentliche Hilfe- und Datenschutzseite zur App **Tauben & Co**
(`de.taubenundco.app`, iPhone und Android).

Google Play verlangt eine öffentlich erreichbare Datenschutz-URL, App Store
Connect zusätzlich eine Support-URL. Die eigentliche Webseite der Vogelstation
(taubenundco.de) liegt hinter einem Anmelde-Tor und kommt dafür nicht in Frage —
deshalb diese Seite über GitHub Pages.

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: was die App ist, die vier Wege, Support-Kontakt |
| `funktionen.html` | Funktionsliste, je Funktion mit Stationstyp (nur Gebautes, Geplantes als „in Arbeit“) |
| `vergleich.html` | BirdNET-Go, BirdNET-Pi + AvianVisitors und Tauben & Co im fairen Vergleich |
| `pi-installieren.html` | Vorschau der Pi-Anleitung (Installer noch in Arbeit) |
| `server-einrichten.html` | Vorschau der Server-Anleitung (Paket noch in Arbeit) |
| `lizenzen.html` | Nennungen und Lizenzen, kostenlos und nicht kommerziell |
| `datenschutz.html` | Datenschutzerklärung (Play: Datenschutz-URL) |
| `stil.css` | gemeinsames Stylesheet der neuen Seiten |
| `.github/ISSUE_TEMPLATE/` | Issue-Formulare: Anbindung vorschlagen, Wunsch, Fehler |
| `.nojekyll` | GitHub Pages soll die Dateien unverändert ausliefern |

Die Quelle von `datenschutz.html` liegt im App-Projekt unter
`app/server/srv/avian/oeffentlich/app/datenschutz.html`. Änderungen gehören
dorthin und werden von hier aus nur kopiert.

Kein Skript, keine fremden Schriften, kein externer Aufruf. Keine Daten aus der
Station: keine Aufnahmen, keine Fundzahlen, keine Standortadressen.

Alle Seiten sind zweisprachig (`<section id="de">`, `<section id="en">`) und haben
oben dieselbe Navigation. Die Seiten außer `datenschutz.html` entstehen aus
`app/github/support-quellen/bauen.py` im App-Projekt (nicht in diesem Repo);
die Funktionsliste steht dort in `inhalt_funktionen.py`. In `datenschutz.html`
steht die Navigation zwischen `<!-- nav:start -->` und `<!-- nav:end -->`: Sie
gehört nur in diese Kopie, nicht in die Quelle am Server. Nach jedem Kopieren der
Quelle `python3 nav-einfuegen.py datenschutz.html` aus `support-quellen/` laufen lassen.
