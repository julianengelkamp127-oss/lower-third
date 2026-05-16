# lower-third

════════════════════════════════════════════════════════════
  ONTIME TECHNIKER-AUSWAHL — INSTALLATIONS-ANLEITUNG
  Jugendkulturnacht 2026
════════════════════════════════════════════════════════════

VORAUSSETZUNGEN
───────────────
  - OnTime läuft auf Port 4001
  - CasparCG Server ist installiert
  - CasparCG Client ist installiert


════════════════════════════════════════════════════════════
  SCHRITT 1 — TECHNIKER-AUSWAHL (index.html)
════════════════════════════════════════════════════════════

Datei:  mm\index.html

Kopieren nach:
  C:\Users\<DEIN-NAME>\AppData\Roaming\ontime\external\mm\

Tipp: Schnell öffnen mit Win+R → eingeben:
  %APPDATA%\ontime\external\mm\

→ Falls der Ordner "mm" nicht existiert: einfach neu erstellen!


════════════════════════════════════════════════════════════
  SCHRITT 2 — LOWER THIRD (CasparCG Template)
════════════════════════════════════════════════════════════

Folgende Dateien kopieren nach:
  C:\Programme\casparcg-server\template\

  ✓ Lower thrid.html
  ✓ scripts\gsap.min.js              (Ordner "scripts" anlegen)
  ✓ media\EncodeSansSemiExpanded-Bold.ttf  (Ordner "media" anlegen)
  ✓ media\HD_ColorBars.svg


════════════════════════════════════════════════════════════
  SCHRITT 3 — ONTIME EINRICHTEN
════════════════════════════════════════════════════════════

1. OnTime öffnen
2. Oben rechts: Settings → View settings
3. Dort muss ein Eintrag existieren:

   Name: mm
   URL:  http://localhost:4001/external/mm/

→ Falls nicht vorhanden: "+ Add" klicken und eintragen


════════════════════════════════════════════════════════════
  SCHRITT 4 — CASPAR EINRICHTEN
════════════════════════════════════════════════════════════

1. CasparCG Server starten
2. CasparCG Client öffnen
3. Links in der Library: "LOWER THRID" auswählen
   (erscheint automatisch wenn die Datei im template-Ordner liegt)
4. In den Inspector-Einstellungen rechts:
   - Server: Localhost
   - Channel: 1
   - Video layer: 20

→ Falls "LOWER THRID" nicht erscheint:
   CasparCG Client neu starten oder Library neu laden


════════════════════════════════════════════════════════════
  TÄGLICHER ABLAUF
════════════════════════════════════════════════════════════

1. OnTime starten
2. Browser öffnen:
   http://localhost:4001/external/mm/
   (oder mit IP: http://192.168.188.187:4001/external/mm/)

3. Passwort eingeben: 1989

4. Person in der Liste auswählen

5. Unten auf "DATEN ÜBERMITTELN" klicken

6. In CasparCG: LOWER THRID → Play drücken
   → Name erscheint auf dem Screen!

7. Zum Ausblenden: Stop drücken


════════════════════════════════════════════════════════════
  SCHNELL-TEST (ist alles korrekt?)
════════════════════════════════════════════════════════════

Nach dem Senden im Browser öffnen:
  http://localhost:4001/api/poll

Dort sollte stehen:
  "secondary": "NAME DER PERSON"
  "timer": { "text": "ROLLE" }

Wenn ja → alles korrekt!
Wenn nein → OnTime neu starten


════════════════════════════════════════════════════════════
  FEHLERBEHEBUNG
════════════════════════════════════════════════════════════

PROBLEM: Seite lädt nicht
  → Ist OnTime gestartet?
  → Stimmt die IP-Adresse? (unten rechts in der Seite änderbar)

PROBLEM: Passwort funktioniert nicht
  → Passwort ist: 1989
  → Seite mit F5 neu laden und nochmal versuchen

PROBLEM: Konzertname zeigt "Lade..."
  → OnTime Projekt-Titel prüfen: Settings → Project data → Title

PROBLEM: Lower Third zeigt "Bandname / Genre"
  → Erst in index.html senden, DANN in Caspar Play drücken
  → Reihenfolge wichtig: Senden → warten → Play

PROBLEM: Lower Third flackert
  → Neueste Version von "Lower thrid.html" verwenden

PROBLEM: Caspar zeigt Template nicht in der Library
  → CasparCG Server neu starten
  → CasparCG Client neu starten

PROBLEM: Offline-Screen erscheint
  → OnTime ist nicht erreichbar
  → OnTime starten und Seite neu laden (F5)


════════════════════════════════════════════════════════════
  PASSWORT ÄNDERN
════════════════════════════════════════════════════════════

In der Datei:
  AppData\Roaming\ontime\external\mm\index.html

Suchen nach:
  const PW = '1989';

Ersetzen mit gewünschtem Passwort, z.B.:
  const PW = 'neuesPasswort';

Datei speichern → fertig!


════════════════════════════════════════════════════════════
  DATEI-ÜBERSICHT
════════════════════════════════════════════════════════════

  mm\index.html                    → Techniker-Auswahl (Browser)
  template\Lower thrid.html        → CasparCG Lower Third
  template\scripts\gsap.min.js     → Animation-Bibliothek
  template\media\*.ttf / *.svg     → Schrift + Logo

════════════════════════════════════════════════════════════
