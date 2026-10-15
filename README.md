# Wetterblick

Eine einzelne lokale HTML-Datei für aktuelle Wetterdaten und eine 5-Tage-Vorhersage.

## Start

`index.html` direkt im Browser öffnen. Für die Wetterabfrage wird eine Internetverbindung benötigt.

Alternativ aus dem Projektordner einen lokalen Server starten:

```bash
python3 -m http.server 8000
```

Dann `http://localhost:8000` öffnen.

## Verwendung

- Ort in das Suchfeld eingeben, z. B. `Berlin`, `New York` oder `Hamburg`.
- Die App ruft im Browser `https://wttr.in/<ORT>?format=j1` ab.
- Es werden keine Konten, API-Schlüssel oder lokalen Server benötigt.

## Projektstruktur

- `index.html` – komplette App mit HTML, CSS und JavaScript
- `README.md` – Dokumentation

## Hinweis zu Netzwerk und Datenschutz

Die Wetterdaten kommen direkt von wttr.in. Beim Absenden einer Suche wird der eingegebene Ort an diesen Dienst übertragen. Die App speichert keine Daten und enthält kein Tracking. Ob der Abruf beim Öffnen per `file://` vom Browser zugelassen wird, hängt von Browser und Umgebung ab; ein lokaler HTTP-Server ist die zuverlässigste Variante.

Datenquelle: [wttr.in](https://wttr.in)
