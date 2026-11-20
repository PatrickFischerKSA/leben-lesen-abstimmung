# LEBEN LESEN – Abstimmung

Statische GitHub-Pages-Oberfläche für die Publikums- und Juryabstimmung des FMS-Kreativprojekts **LEBEN LESEN**.

- Öffentliche Abstimmung: `index.html`
- Juryzugang: `?jury`
- Abstimmungsregie: `?admin`
- Datenhaltung: Cloudflare Worker + D1 der Projektplattform

Die Seite speichert keine Passwörter und keine Ergebnisse im GitHub-Repository. Gerätekennungen werden im Browser erzeugt und vom Backend nur als HMAC-Hash gespeichert. E-Mail-Adressen der Jury werden nicht persistiert und nicht in Sitzungstokens übernommen; jede Juryanmeldung erhält stattdessen ein zufälliges, nicht zuordenbares Sitzungspseudonym. Jurywerte werden beim Absenden unmittelbar zu Summen addiert und nicht als Einzelstimmen gespeichert. Dashboard und Export enthalten ausschliesslich diese aggregierten Werte.
