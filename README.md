# Hau den Erdi! 🔨

Ein Whack-a-Mole-Spiel im Cartoon-Stil für das iPhone: Erdmännchen schauen aus ihren Löchern, du haust sie mit dem Hammer.

- **Erdmännchen**: +10 Punkte
- **Erdmännchen mit Helm**: zweimal hauen, +5 und +25 Punkte
- **Igel**: Finger weg! −20 Punkte und Serie weg
- **Serie**: je 5 Treffer in Folge erhöhen den Multiplikator (bis ×5). Daneben tippen oder ein Erdmännchen entwischen lassen setzt die Serie zurück.
- Das Spiel dauert 45 Sekunden und wird gegen Ende schneller. Der Rekord wird lokal im Browser gespeichert.

## Spielen

Das Spiel besteht nur aus `index.html` (kein Build, keine Abhängigkeiten).

**Mit GitHub Pages hosten:** Repo → *Settings → Pages → Deploy from a branch* → Branch wählen, Ordner `/ (root)`. Die URL in Safari öffnen.

**Als App auf den Home-Bildschirm:** in Safari *Teilen → Zum Home-Bildschirm*. Dann läuft es im Vollbild ohne Adressleiste.

## Hinweise

- Ton: iOS spielt Web-Audio nur nach der ersten Berührung ab. Der Stumm-Schalter am Gerät kann den Ton trotzdem stumm halten.
- Haptik: Safari auf dem iPhone unterstützt `navigator.vibrate` nicht. Das Spiel nutzt deshalb einen unsichtbaren `<input switch>`, der in neueren iOS-Versionen einen Tick auslösen kann. Das ist nicht auf einem echten Gerät geprüft.
