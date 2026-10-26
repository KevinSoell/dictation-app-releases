# Dictation App (macOS)

Lokale Diktier-App für Macs mit Apple-Chip (M1 oder neuer), macOS 14 oder neuer.
Die Spracherkennung läuft vollständig auf dem Mac, ohne Konto, Abo oder Cloud.

**Download:** [Dictation-App.dmg](https://github.com/KevinSoell/dictation-app-releases/releases/latest/download/Dictation-App.dmg)

1. DMG öffnen, **Dictation App** auf **Applications** ziehen.
2. Dictation App starten. Beim ersten Start meldet macOS, dass die App nicht überprüft
   werden kann (sie ist privat signiert): **Fertig** → Systemeinstellungen →
   Datenschutz & Sicherheit → bei „Dictation App“ **Dennoch öffnen** (je nach macOS „Trotzdem öffnen“).
3. Im Willkommensfenster Mikrofon und Bedienungshilfen erlauben; das Sprachmodell
   (ca. 600 MB) lädt einmalig.

Updates installieren sich danach automatisch (nie während einer Aufnahme).

## Datenschutz (kurz)

- Aufnahmen, Texte, History, Wörterbuch und Einstellungen bleiben auf deinem Mac
  (`~/Library/Application Support/DictationApp`); es gibt kein Konto, keine
  Telemetrie und keine Cloud-Transkription. Aufnahmen werden standardmäßig nach
  7 Tagen gelöscht (Settings → Privacy).
- Netzwerk nutzt die App nur für zwei Dinge: den einmaligen Download des
  Sprachmodells von Hugging Face und die tägliche Update-Prüfung bei GitHub. Dabei
  sehen diese Dienste – wie bei jedem Download – deine IP-Adresse und die App-Version,
  nichts von deinen Diktaten.
- Sicherheitsprobleme bitte über [SECURITY.md](SECURITY.md) melden.

Dieses Repository enthält nur fertige, signierte Downloads und den Update-Feed –
keinen Quellcode. Drittanbieter-Hinweise: `Acknowledgements.txt` in der App
(Sprachmodell Parakeet Ultra von moondream auf Basis von NVIDIA parakeet-tdt-0.6b-v3,
CC-BY-4.0; Sparkle, MIT; FluidAudio, Apache-2.0; WhisperKit, MIT).
