# Spielerei 🎮

Kleine Spiele fürs iPhone, jedes als einzelne HTML-Datei ohne Build und ohne Abhängigkeiten.

| Spiel | Ordner | Beschreibung |
|---|---|---|
| Hau den Erdi! | [`hau-den-erdi/`](hau-den-erdi/) | Cartoon-Whack-a-Mole: Erdmännchen hauen, Helme knacken, Igel verschonen |

Die Startseite (`index.html`) listet alle Spiele. Live: https://benjaminra-art.github.io/Spielerei/

## Auf dem iPhone spielen

Die Seite oder ein einzelnes Spiel in Safari öffnen, dann *Teilen → Zum Home-Bildschirm*. Jedes Spiel hat ein eigenes Icon und läuft im Vollbild.

## Neues Spiel hinzufügen

1. Ordner anlegen, z. B. `mein-spiel/`, mit `index.html` und `apple-touch-icon.png` (180×180).
2. Im Browser-Speicher (`localStorage`) einen **eigenen Präfix** verwenden (z. B. `meinspiel-best`). Alle Spiele laufen auf derselben Domain und teilen sich den Speicher.
3. In der Startseite `index.html` eine Karte ergänzen.

## Hinweis

Dieses Repo ist öffentlich. Alles, was hier liegt, auch Entwürfe und die Git-Historie, ist für jeden sichtbar.

## Hau den Erdi!

- **Erdmännchen**: +10 Punkte
- **Erdmännchen mit Helm**: zweimal hauen, +5 und +25 Punkte
- **Igel**: Finger weg! −20 Punkte und Serie weg
- **Serie**: je 5 Treffer in Folge erhöhen den Multiplikator (bis ×5). Daneben tippen oder ein Erdmännchen entwischen lassen setzt die Serie zurück.
- 45 Sekunden, wird gegen Ende schneller. Der Rekord wird lokal im Browser gespeichert.
- Ton startet erst nach der ersten Berührung. Der Stumm-Schalter am iPhone kann ihn stumm halten.
- Haptik: Safari auf dem iPhone kennt `navigator.vibrate` nicht. Das Spiel nutzt einen unsichtbaren `<input switch>` als Umweg. Das ist nicht auf einem echten Gerät geprüft.
