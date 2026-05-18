════════════════════════════════════════════════════════════
  LOWER THIRDS FOR ONTIME
  by Julian Engelkamp & Jan Rockahr  ·  © Red-Uhu Broadcast
════════════════════════════════════════════════════════════


════════════════════════════════════════════════════════════
  SCHRITT 1 — DATEIEN KOPIEREN
════════════════════════════════════════════════════════════

  index.html  →  AppData\Roaming\ontime\external\mm\index.html

  Schnell öffnen: Win+R → eingeben:
    %APPDATA%\ontime\external\mm\

  Falls Ordner "mm" nicht existiert: neu erstellen!

  ──────────────────────────────────────────────────────────

  Lower thrid.html  →  C:\Programme\casparcg-server\template\
  scripts\gsap.min.js   →  C:\Programme\casparcg-server\template\scripts\
  media\*.ttf / *.svg   →  C:\Programme\casparcg-server\template\media\


════════════════════════════════════════════════════════════
  SCHRITT 2 — ONTIME EINRICHTEN
════════════════════════════════════════════════════════════

  1. OnTime öffnen
  2. Settings → View settings
  3. Eintrag muss vorhanden sein:
       Name: mm
       URL:  http://localhost:4001/external/mm/
  4. Falls nicht: "+ Add" klicken und eintragen


════════════════════════════════════════════════════════════
  SCHRITT 3 — CUSTOM FIELDS IN ONTIME EINRICHTEN
════════════════════════════════════════════════════════════

  Settings → Project settings → Custom fields

  Folgende Felder werden empfohlen:

  GENRE
  ─────
  Feldname: Gernre   (ACHTUNG: Tippfehler — so lassen!)
  Inhalt:   Musikgenre der Band, z.B. Rock, Pop, Tanz, HipHop
  Hinweis:  Erscheint als zweite Zeile im Lower Third (f1)

  CREW
  ────
  Stagemanager     → Name des Stagemanagers
  Licht            → Lichttechniker
  Schnitt          → Schnitttechniker
  Ton_FOH          → Tontechniker
  Kamera_Links     → Kamera Links
  Kamera_Rechts    → Kamera Rechts
  Kamera_Hinten    → Kamera Hinten
  Produzent        → Produzent
  Streamton        → Streamton-Techniker

  BAND-INSTRUMENTE
  ────────────────
  Gesang           → Sänger / Sängerin
  Begleitgesang    → Backing Vocals
  Gitarre          → Gitarrist
  Akustikgitarre   → Akustikgitarrist
  Bass             → Bassist
  Schlagzeug       → Schlagzeuger
  Percussion       → Percussionist
  Keyboard         → Keyboarder
  Piano / Klavier  → Pianist
  Violine / Geige  → Geiger
  Mandoline        → Mandolinenspieler
  Ukulele          → Ukulelenspieler
  Saxophon         → Saxophonist
  Trompete         → Trompeter
  Dudelsack        → Dudelsackspieler
  Mundharmonika    → Mundharmonikaspieler
  Floete           → Flötist
  Querfloete       → Querflötist

  VEREIN
  ──────
  Vereinsmitglied    → Name des Vereinsmitglieds
                       erscheint in der Liste mit Rolle "Vereinsmitglied"
  Vorstandsmitglied  → Name des Vorstandsmitglieds
                       erscheint in der Liste mit Rolle "Vorstandsmitglied"


════════════════════════════════════════════════════════════
  SCHRITT 4 — CASPAR EINRICHTEN
════════════════════════════════════════════════════════════

  1. CasparCG Server starten
  2. CasparCG Client öffnen
  3. Links in der Library: "LOWER THRID" auswählen
  4. Inspector rechts:
       Server:      Localhost
       Channel:     1
       Video layer: 20

  Falls "LOWER THRID" nicht erscheint:
  → CasparCG Server + Client neu starten


════════════════════════════════════════════════════════════
  TÄGLICHER ABLAUF
════════════════════════════════════════════════════════════

  1. OnTime starten

  2. Browser öffnen:
       http://localhost:4001/external/mm/
     (oder mit IP: http://192.168.188.187:4001/external/mm/)

  3. Passwort eingeben: 1989

  4. Person in der Liste auswählen

  5. "DATEN ÜBERMITTELN" klicken

  6. In CasparCG: LOWER THRID → Play drücken
     → Name + Genre/Rolle erscheint auf dem Screen!

  7. Zum Ausblenden: Stop drücken

  !! WICHTIG: Erst senden, DANN Play drücken !!


════════════════════════════════════════════════════════════
  FILTER IN DER LISTE
════════════════════════════════════════════════════════════

  ALLE         → Alle Personen anzeigen
  BAND         → Nur Bandnamen (Event-Titel aus OnTime)
  CREW         → Nur Technik-Personal
  STAGEMANAGER, KAMERA, TON, LICHT, SCHNITT, PRODUKTION
               → Direkte Rollenfilter

  ▼ Alle Rollen → Weitere Rollen ausklappen
    (Instrumente, Vereinsmitglied, Vorstandsmitglied...)


════════════════════════════════════════════════════════════
  WAS ERSCHEINT IM LOWER THIRD?
════════════════════════════════════════════════════════════

  f0 (oben, groß)   = Name der Person / Band
  f1 (unten, klein) = Genre oder Rolle

  Beispiele:
    HIPHOP GIRLS RECKLINGHAUSEN / Tanz
    JULIAN / Stagemanager
    ABANDONED HEAVEN / Rock
    SINA / Kamera
    MAX MUSTERMANN / Vereinsmitglied

  Band ohne Genre eingetragen → zeigt "Band"
  Crew-Mitglied → zeigt die Rolle


════════════════════════════════════════════════════════════
  PASSWORT ÄNDERN
════════════════════════════════════════════════════════════

  In: AppData\Roaming\ontime\external\mm\index.html

  Zeile suchen:   const PW = '1989';
  Ersetzen mit:   const PW = 'neuesPasswort';


════════════════════════════════════════════════════════════
  IP-ADRESSE ÄNDERN (neuer PC)
════════════════════════════════════════════════════════════

  Seite öffnen → unten rechts im Server-Feld
  neue IP eingeben → Enter oder ↺ Verbinden drücken
  IP wird automatisch gespeichert (bleibt auch nach F5)


════════════════════════════════════════════════════════════
  FEHLERBEHEBUNG
════════════════════════════════════════════════════════════

  Seite lädt nicht
  → OnTime gestartet? IP korrekt?

  Passwort falsch
  → Passwort ist: 1989

  Konzertname zeigt "Lade..."
  → OnTime → Settings → Project data → Project title prüfen

  Lower Third zeigt "Bandname / Genre"
  → Erst senden, DANN Play in Caspar!

  Genre wird nicht angezeigt
  → Feld heißt "Gernre" (Tippfehler in OnTime) — so lassen!
  → Kein Genre eingetragen → zeigt automatisch "Band"

  OFFLINE-Screen erscheint
  → OnTime starten, dann F5

  Caspar zeigt Template nicht
  → CasparCG Server + Client neu starten

  Beim Band-Filter erscheinen Bandmitglieder
  → In index.html prüfen ob diese Zeile vorhanden ist:
     if (activeRoleFilter === 'band') return t.isBandTitle === true;


════════════════════════════════════════════════════════════
  DATEI-ÜBERSICHT
════════════════════════════════════════════════════════════

  mm\index.html                    → Browser (OnTime-Seite)
  template\Lower thrid.html        → CasparCG Template
  template\scripts\gsap.min.js     → Animation
  template\media\*.ttf / *.svg     → Schrift + Grafik

════════════════════════════════════════════════════════════
