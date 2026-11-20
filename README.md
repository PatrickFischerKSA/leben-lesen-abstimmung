# LEBEN LESEN – Abstimmung

Statische GitHub-Pages-Oberfläche für die Publikums- und Juryabstimmung des FMS-Kreativprojekts **LEBEN LESEN**.

- Öffentliche Abstimmung: `index.html`
- Juryzugang: `?jury`
- Abstimmungsregie: `?admin`
- Datenhaltung: Cloudflare Worker + D1 der Projektplattform

Die Seite speichert keine Passwörter und keine Ergebnisse im GitHub-Repository. Gerätekennungen werden im Browser erzeugt und vom Backend nur als HMAC-Hash gespeichert.
