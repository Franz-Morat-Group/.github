<!--
  Org-Profil-README  →  gehört nach:  .github/profile/README.md
  Vor dem Commit anzupassen: Logo-Asset unter profile/assets/, Repo-Tabelle, Kontakt-Mail.
-->

<div align="center">

<img src="profile/assets/framo-morat-logo.png" alt="Framo Morat" width="220">

# Framo Morat

**Franz Morat Group · Antriebstechnik aus dem Hochschwarzwald**
Interne und öffentliche Software-Tools rund um Zahnräder, Getriebe und Antriebssysteme.

[![Design Guideline](https://img.shields.io/badge/Design%20Guideline-lesen-2f92dd?style=flat&labelColor=141a24)](https://github.com/Franz-Morat-Group/design-guideline)
[![Framo Morat](https://img.shields.io/badge/Industrie-Framo%20Morat-a9b4c2?style=flat&labelColor=141a24)](https://framo-morat.com)
[![F. Morat](https://img.shields.io/badge/Automotive-F.%20Morat-a9b4c2?style=flat&labelColor=141a24)](https://f-morat.com)
[![Franz Morat Group](https://img.shields.io/badge/Gruppe-franz--morat.com-a9b4c2?style=flat&labelColor=141a24)](https://franz-morat.com)

</div>

---

## Wer wir sind

**Framo Morat** entwickelt und fertigt hochpräzise Zahnräder, Getriebekomponenten und komplette Antriebssysteme für die Industrie – von Automatisierung und Intralogistik über Medizin- und Rehatechnik bis zu erneuerbaren Energien und Landtechnik. Zusammen mit **F. Morat** (Automotive) bildet Framo Morat die **Franz Morat Group** mit Stammsitz in Eisenbach im Hochschwarzwald.

| Kennzahl | Wert |
|---|---:|
| Erfahrung Metallverarbeitung | über 110 Jahre |
| Mitarbeitende | über 700 |
| Umsatz | rund 115 Mio. € |
| Tochterfirmen | USA, Polen, Mexiko, Türkei |

---

## Was in dieser Organisation liegt

Web-basierte Engineering- und Auswertungs-Tools, Berechnungs-Rechner und interne Automatisierung. Der überwiegende Teil der Repositories ist privat.

<!-- Repo-Tabelle hier pflegen; keine Platzhalter-Zeilen im Live-Stand stehen lassen. -->

| Repository | Zweck | Status |
|---|---|---|
| [`design-guideline`](https://github.com/Franz-Morat-Group/design-guideline) | Verbindliche Frontend Design Guideline + `design-tokens.css` | aktiv |
| [`screw-study`](https://github.com/Franz-Morat-Group/screw-study) | Anzieh-Drehmoment-Auswertung, Referenz-Implementierung der Guideline | aktiv |

---

## Frontend Design Guideline

Jedes Tool sieht aus wie aus einem Guss – unabhängig davon, wer oder was es gebaut hat. Verbindlich für alle Frontends in dieser Organisation:

- **Dark Mode ist Standard.** Helles Theme nur für öffentliche/Marketing-nahe Seiten.
- **Nur Tokens.** Farben, Schrift, Radius und Abstände ausschließlich aus `design-tokens.css` – keine frei erfundenen Hex-Werte oder Pixelgrößen.
- **System-Font-Stack.** Keine Custom Fonts; Neuzeit Grotesk bleibt Print und Marketing.
- **Layout.** Sticky Topbar, feste Sidebar (~330 px) für Eingaben und Parameter, Hauptbereich mit Tabs, Breakpoint bei ~1080 px auf einspaltig.
- **Genau ein `btn-primary`** pro Ansicht, alles andere `btn` / `btn-ghost` / `btn-mini`.
- **Diagramme als eigenes SVG**, ohne Chart-Bibliothek. Farben zur Laufzeit aus den CSS-Variablen lesen, Hover als Crosshair mit Wert-Readout statt Tooltip-Popup.
- **Status ist fix verdrahtet.** `--bad` ist überall Rot; Statusfarben werden nie mit Markenfarben verwechselt.

### Token-Kern

| Rolle | Wert | Verwendung |
|---|---|---|
| `--brand-blue` | `#0069b4` | Framo Morat, Branding-Flächen |
| `--brand-grey` | `#575756` | Franz Morat Group, neutral |
| `--brand-green` | `#005a44` | F. Morat, ausschließlich Automotive-Tools |
| `--accent` | `#2f92dd` | Einzige Interaktionsfarbe |
| `--bg` / `--panel` | `#0b0f16` / `#141a24` | Seite / Karten |
| `--text` / `--text-dim` / `--muted` | `#e6edf3` / `#a9b4c2` / `#7d8899` | Text-Hierarchie |
| `--ok` / `--warn` / `--bad` / `--info` | `#3fb950` / `#e3b341` / `#f85149` / `#58a6ff` | Status |
| `--radius` / `--radius-sm` | `10px` / `6px` | Panels / Buttons und Inputs |

Vollständige Regeln, Komponenten-Patterns und der kopierbare Token-Block: **[design-guideline](https://github.com/Franz-Morat-Group/design-guideline)**.

<details>
<summary><b>Baustein für AI-Coding-Prompts</b> (Claude, Cursor, Copilot)</summary>

> Baue die UI dunkel (Dark Mode als Standard) und nutze ausschließlich die CSS Custom Properties aus `design-tokens.css` (Franz Morat Group Design Guideline) für Farben, Schrift, Radius und Abstände – keine frei erfundenen Hex-Werte oder Pixelgrößen. Interaktionsfarbe ist `--accent` (aufgehelltes Markenblau), Statusfarben `--ok`/`--warn`/`--bad`/`--info` sind fix verdrahtet und nicht mit Markenfarben zu verwechseln. Schrift ist der System-Font-Stack, keine Custom Fonts laden. Radius: 10px für Panels/Karten, 6px für Buttons/Inputs, 999px nur für Badges. Layout: sticky Topbar, feste Sidebar (~330px) für Eingaben/Parameter, Hauptbereich mit Tabs für Ergebnisse, Breakpoint bei ~1080px auf einspaltig. Diagramme als eigenes SVG (keine Chart-Bibliothek), Farben zur Laufzeit aus den CSS-Variablen lesen, Achsen mit gerundeten Ticks, Hover als Crosshair mit Wert-Readout statt Tooltip. Tabellen: Zahlen rechtsbündig mit tabular-nums, Status als 3px linker Zeilenrahmen statt Volltonhintergrund. Badges immer als Pill mit softem (13%) Farbhintergrund statt Vollton. Genau ein `btn-primary` pro Ansicht, alle anderen Aktionen `btn`/`btn-ghost`/`btn-mini`.

</details>

---

## Neues Tool starten

1. `design-tokens.css` aus dem Guideline-Repo übernehmen und global einbinden.
2. Layout-Grundgerüst aufsetzen: Topbar (Logo-Kachel, Titel, Subtitle, Status), Sidebar für Input, Tabs für Ergebnisse.
3. Empty State vor dem ersten Ergebnis, Toast für Rückmeldungen, keine blockierenden Modals.
4. Vor dem Merge gegen den Abschnitt „Nicht erlaubt“ der Guideline prüfen.

## Konventionen

- **Repo-Namen:** `kebab-case`, Sache statt Abteilung – z. B. `screw-study`, nicht `tool-qs-2`.
- **Commits:** Conventional Commits (`feat:`, `fix:`, `refactor:`, `docs:`).
- **Branches:** kurzlebige Feature-Branches, Merge über Pull Request in `main`.
- **Keine Geheimnisse und keine Kundendaten im Repo** – auch nicht in Testdaten, Screenshots oder Beispiel-Konfigurationen.

## Kontakt

Fragen zu Repos oder Tools dieser Organisation: **it@franz-morat.com** · Allgemeine Anfragen über [franz-morat.com](https://franz-morat.com)

<div align="center">
<sub>Franz Morat Group · Eisenbach im Hochschwarzwald · Ihre Idee – Unser Antrieb</sub>
</div>
