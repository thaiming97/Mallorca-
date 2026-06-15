# WM 2026 · Tippspiel

Ein vollständig clientseitiges Fußball-Tippspiel als statische Website – kein
Server, kein Build-Tool, keine Abhängigkeiten. Einfach `index.html` im Browser
öffnen.

## Funktionen

- **Spieler verwalten** – Mitspieler hinzufügen und entfernen.
- **Tippen** – pro Spieler ein Ergebnis je Partie tippen.
- **Ergebnisse eintragen** – echte Endergebnisse erfassen.
- **Rangliste** – Punkte werden automatisch berechnet und sortiert.
- **Speichern** – alle Daten liegen lokal im Browser (`localStorage`).
- **Export / Import** – Spielstand als JSON-Datei sichern und wieder laden.

## Punkteregeln

| Tipp                          | Punkte |
|-------------------------------|:------:|
| Exaktes Ergebnis              |   3    |
| Richtige Tendenz (Sieg/Remis) |   1    |
| Daneben                       |   0    |

Sobald für eine Partie ein Ergebnis eingetragen ist, wird der Tipp gesperrt und
die erreichten Punkte direkt angezeigt.

## Spielplan anpassen

Der Beispiel-Spielplan steht in `index.html` in der Konstante
`DEFAULT_MATCHES`. Dort lassen sich Begegnungen, Flaggen-Emojis und Termine
beliebig ändern oder ergänzen.

## Nutzung

```
tippspiel/index.html  →  im Browser öffnen
```

Läuft komplett offline.
