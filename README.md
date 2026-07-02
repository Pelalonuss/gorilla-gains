# Gorilla Gains 🦍💦

Ein knallbunter **Beast-Mode Trainings-Tracker** im Neon-/Comic-Look – mit Dopamin-Konfetti,
automatischem Pausen-Timer und Fortschritts-Verlauf. Läuft komplett im Browser, ohne Account,
alle Daten bleiben auf deinem Gerät. Als **PWA** installierbar direkt auf dem iPhone-Home-Bildschirm.

👉 **Live:** **https://pelalonuss.github.io/gorilla-gains/**

---

## Features

- 🏋️ **Training-Tracker** – Sätze abhaken, Gewicht & Reps direkt eintragen, Live-Volumen & Fortschrittsbalken
- ⏱️ **Auto-Pausentimer** – startet automatisch beim Abhaken eines Satzes, mit ±15s, Pause/Weiter, Ton & (Android-)Vibration
- 📈 **„Letztes Mal"-Anzeige** pro Übung für sauberes progressives Überladen
- 📊 **Verlauf & Statistik** – Streak 🔥, Workouts diese Woche, Gesamt-Volumen, Verlaufsbalken der letzten 10 Einheiten
- 📝 **Planer** – Trainingstage anlegen, Übungen hinzufügen/sortieren, Sätze/Reps/Pause pro Übung, Farbe wählen
- 🎉 **Dopamin-Konfetti** bei jedem Satz und ein Mega-Feuerwerk am Ende
- 💾 **Backup & Import** als JSON, plus komplettes Zurücksetzen
- ☀️ **Wake-Lock** – Bildschirm bleibt während des Trainings an
- 📲 **PWA** – installierbar, läuft offline (nach dem ersten Laden), Vollbild ohne Browser-Leiste

## Auf dem iPhone installieren

1. Die Live-URL in **Safari** öffnen.
2. Unten auf das **Teilen-Symbol** ⬆️ tippen.
3. **„Zum Home-Bildschirm"** wählen → fertig. Das Gorilla-Icon erscheint wie eine echte App.

Danach startet Gorilla Gains im Vollbild und funktioniert auch offline.

## Technik

- Single-File React (18) via CDN, in-browser mit Babel kompiliert (klassischer JSX-Runtime)
- Tailwind CSS (CDN) fürs Styling, `canvas-confetti` für den Dopamin-Kick
- `localStorage` für alle Daten, Service Worker für Offline-Betrieb
- Keine Build-Tools, kein Backend, kein Tracking

## Lokal starten

Einfach `index.html` mit einem kleinen Webserver ausliefern (Service Worker braucht `http`/`https`, nicht `file://`):

```bash
python -m http.server 5173
# dann http://localhost:5173 öffnen
```

## Daten & Privatsphäre

Alles wird ausschließlich lokal im Browser gespeichert. Es werden keine Daten an einen Server gesendet.
Wenn du den Browser-Speicher löschst, sind die Daten weg – deshalb gibt es unter **Setup → Backup** einen Export.

---

Made with 🦍 & 💦 – Beast Mode on.
