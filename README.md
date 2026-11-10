# treueturbo-site

Statische Website für den Treue-Turbo (Locadas GmbH). Drei Dateien, kein Build.

- `index.html` Startseite
- `impressum.html` Impressum
- `datenschutz.html` Datenschutz

## Vor dem Livegang

1. Calendly-Link in `index.html` eintragen: Zeile mit `var CALENDLY=''`.
2. Sobald Calendly genutzt wird: in `datenschutz.html` den Abschnitt „Gespräch vereinbaren“ um Calendly ergänzen.
3. Datenschutz einmal rechtlich gegenlesen lassen.

## Weg A: GitHub Pages mit IONOS-Domain

1. Repository auf GitHub anlegen und diese Dateien pushen.
2. Im Repository unter Settings, Pages: Branch `main`, Ordner `/ (root)`.
3. Unter Custom domain die Domain eintragen, zum Beispiel `treueturbo.de`. GitHub legt dann die Datei `CNAME` an.
4. Bei IONOS unter Domains, DNS:
   - vier A-Einträge für `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - ein CNAME-Eintrag für `www` auf `<github-name>.github.io`
   - vorhandene A- und AAAA-Einträge für `@` vorher entfernen
5. Warten, bis GitHub die Domain bestätigt, dann „Enforce HTTPS“ aktivieren.

## Weg B: IONOS-Webspace

Die drei Dateien per SFTP oder über den Dateimanager in das Verzeichnis der Domain laden. Fertig.
