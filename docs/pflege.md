# Profilseite lokal pflegen

`index.html` enthält die Texte, Links und das CSS der Seite. Das Profilbild liegt in `avatar.webp`, das Tab-Symbol in `favicon.svg`. Beim Ersetzen unter neuem Namen auch den relativen Pfad im HTML aktualisieren. Der Alternativtext des Bildes sollte weiterhin zum dargestellten Motiv passen.

## Vorschau

Im Repository-Stamm starten und im Browser [die lokale Vorschau](http://127.0.0.1:8000/) öffnen.

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

1. Profilbild und Tab-Symbol prüfen. Unter `/avatar.webp` und `/favicon.svg` können die beiden Dateien auch einzeln geöffnet werden.
2. Nach dem Neuladen **Tab** drücken. **Zum Inhalt springen** sollte sichtbar werden. Mit **Enter** zum Hauptinhalt springen.
3. Mit **Tab** eine Gruppenüberschrift ansteuern. **Enter** öffnet das native `details`-Element. **Leertaste** auf der fokussierten Überschrift schließt es wieder.
4. Bei schmalem Browserfenster kontrollieren, dass Linktexte lesbar bleiben und der Tastaturfokus sichtbar ist. Für die lokale Prüfung genügt es, die Links zu fokussieren.

## Links ändern

Jede Gruppe besteht aus `details`, einer Überschrift in `summary` und den zugehörigen Links. Bei einem neuen oder entfernten Link auch die sichtbare Anzahl und das zugehörige `aria-label` in `summary` anpassen. Bei einem umbenannten Ziel sichtbaren Namen und vorhandene Zugänglichkeitsbeschriftung gemeinsam prüfen. Der Sprunglink verweist auf `#main-content` im selben Dokument.
