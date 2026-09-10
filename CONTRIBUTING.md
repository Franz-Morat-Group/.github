# Beitragen

Danke, dass du zu einem Repository der **Franz Morat Group** beiträgst. Diese
Richtlinie gilt organisationsweit für alle Repos, sofern ein Repository keine
eigene, spezifischere `CONTRIBUTING.md` mitbringt.

Mit deinem Beitrag akzeptierst du unseren
[Verhaltenskodex](CODE_OF_CONDUCT.md).

## Grundregeln

- **Vertraulichkeit:** Die meisten Repos sind privat. Keine vertraulichen
  Inhalte, Zugangsdaten, Schlüssel oder personenbezogenen Daten in Code,
  Commits, Issues oder Testdaten.
- **Design Guideline:** Frontend-Arbeit richtet sich nach der verbindlichen
  [Design Guideline](https://github.com/Franz-Morat-Group/design-guideline)
  und nutzt die zentrale `design-tokens.css`. Als Referenz-Implementierung
  dient [`screw-study`](https://github.com/Franz-Morat-Group/screw-study).
- **Fragen?** Ansprechpartner findest du in [SUPPORT.md](SUPPORT.md).

## Ablauf

1. **Issue zuerst:** Für Bugs und Ideen bitte zunächst ein Issue über die
   [Vorlagen](.github/ISSUE_TEMPLATE) anlegen – so vermeiden wir Doppelarbeit und
   klären den Rahmen.
2. **Branch anlegen:** Arbeite in einem eigenen Branch, nicht direkt auf
   `main`.
   - Namensschema: `feature/kurzbeschreibung`, `fix/kurzbeschreibung`,
     `docs/kurzbeschreibung`.
3. **Umsetzen:** Kleine, nachvollziehbare Commits. Bestehende Code- und
   Ordnerstrukturen des jeweiligen Repos beibehalten.
4. **Pull Request öffnen:** Gegen `main`, mit ausgefülltem
   [PR-Template](.github/PULL_REQUEST_TEMPLATE.md). Verweise auf das zugehörige Issue
   (`Closes #123`).
5. **Review:** Mindestens eine Freigabe abwarten. Rückfragen sachlich klären,
   dann wird gemergt.

## Commit-Nachrichten

- Kurze, prägnante Betreffzeile im Imperativ (z. B. „Fix Drehmoment-Berechnung
  bei M8").
- Bei Bedarf ein kurzer Textkörper mit dem *Warum* der Änderung.
- Deutsch oder Englisch – innerhalb eines Repos einheitlich.

## Qualität

- Vor dem PR lokal prüfen, dass alles baut/läuft und keine offensichtlichen
  Fehler bestehen.
- Änderungen an der Oberfläche gegen die Design Guideline gegenprüfen
  (Tokens statt fester Farben/Abstände, konsistente Komponenten).
- Dokumentation (README o. ä.) bei relevanten Änderungen mitpflegen.

## Sicherheit

Sicherheitsrelevante Probleme **nicht** öffentlich als Issue melden, sondern
vertraulich gemäß [SECURITY.md](SECURITY.md).

---

<sub>Fragen zum Ablauf? → [SUPPORT.md](SUPPORT.md)</sub>
