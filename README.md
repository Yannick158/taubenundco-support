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
| `impressum.html` | Impressum nach § 18 Abs. 1 MStV (Handarbeit, wird vom Generator nie überschrieben) |
| `stil.css` | gemeinsames Stylesheet der neuen Seiten |
| `.github/ISSUE_TEMPLATE/` | Issue-Formulare: Anbindung vorschlagen, Wunsch, Fehler |
| `.nojekyll` | GitHub Pages soll die Dateien unverändert ausliefern |

`datenschutz.html` und `impressum.html` sind Handarbeit und werden direkt in
diesem Repo gepflegt. Die Vogelanzeige leitet `/app/datenschutz.html` auf diese
Seite um; es gibt also nur eine Fassung der Datenschutzerklärung.

Kein Skript, keine fremden Schriften, kein externer Aufruf. Keine Daten aus der
Station: keine Aufnahmen, keine Fundzahlen, keine Standortadressen.

Alle Seiten sind zweisprachig (`<section id="de">`, `<section id="en">`) und haben
oben dieselbe Navigation. Die Seiten außer `datenschutz.html` und `impressum.html` entstehen aus
`app/github/support-quellen/bauen.py` im App-Projekt (nicht in diesem Repo);
die Funktionsliste steht dort in `inhalt_funktionen.py`. Die Navigation in
`datenschutz.html` erneuert `nav-einfuegen.py` aus demselben Ordner. Die Seiten
enthalten keine HTML-Kommentare.
