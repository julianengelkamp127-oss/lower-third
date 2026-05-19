════════════════════════════════════════════════════════════
  LOWER THIRDS FOR ONTIME
  by Julian Engelkamp & Jan Rockahr  ·  © Red-Uhu Broadcast
════════════════════════════════════════════════════════════


════════════════════════════════════════════════════════════
  SCHRITT 1 — DATEIEN KOPIEREN
════════════════════════════════════════════════════════════

  index.html  →  AppData\Roaming\ontime\external\mm\index.html

  Schnell öffnen mit Win+R → eingeben:
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
  SCHRITT 3 — CUSTOM FIELDS IN ONTIME
════════════════════════════════════════════════════════════

  Settings → Project settings → Custom fields

  GENRE (wichtig für Bands!)
  ──────────────────────────
  Feldname: Gernre   ← TIPPFEHLER absichtlich so lassen!
  Inhalt:   Rock, Pop, Tanz, HipHop, etc.
  → Erscheint als zweite Zeile im Lower Third

  CREW
  ────
  Stagemanager     Licht            Schnitt
  Ton_FOH          Ton_stream       Kamera_Links
  Kamera_Rechts    Kamera_Hinten    Produzent

  INSTRUMENTE (Band-Mitglieder)
  ──────────────────────────────
  Gesang           Begleitgesang    Gitarre
  Akustikgitarre   Bass             Schlagzeug
  Percussion       Keyboard         Piano / Klavier
  Violine / Geige  Mandoline        Ukulele
  Saxophon         Trompete         Dudelsack
  Mundharmonika    Floete           Querfloete

  VEREIN
  ──────
  Vereinsmitglied    → erscheint mit Rolle "Vereinsmitglied"
  Vorstandsmitglied  → erscheint mit Rolle "Vorstandsmitglied"


════════════════════════════════════════════════════════════
  SCHRITT 4 — CASPAR EINRICHTEN
════════════════════════════════════════════════════════════

  1. CasparCG Server starten
  2. CasparCG Client öffnen
  3. Library links: "LOWER THRID" auswählen
  4. Inspector rechts:
       Server:      Localhost
       Channel:     1
       Video layer: 20

  Falls "LOWER THRID" nicht in der Library erscheint:
  → CasparCG Server + Client komplett neu starten


════════════════════════════════════════════════════════════
  TÄGLICHER ABLAUF
════════════════════════════════════════════════════════════

  1. OnTime starten

  2. Browser öffnen (PC oder Handy im gleichen WLAN!):
       http://localhost:4001/external/mm/
     oder mit IP:
       http://192.168.188.187:4001/external/mm/

  3. Passwort: 1989

  4. Person in der Liste auswählen

  5. "DATEN ÜBERMITTELN" klicken

  6. CasparCG: LOWER THRID → Play
     → Name + Genre/Rolle erscheint auf dem Bildschirm!

  7. Ausblenden: Stop

  !! WICHTIG: Erst senden, DANN Play drücken !!


════════════════════════════════════════════════════════════
  HANDY-NUTZUNG
════════════════════════════════════════════════════════════

  Die Seite funktioniert auch auf dem Handy!

  Voraussetzung: Handy und OnTime-PC im gleichen WLAN

  URL im Handy-Browser eingeben:
    http://192.168.188.187:4001/external/mm/
    (IP anpassen falls nötig — steht unten rechts auf der Seite)

  Passwort: 1989

  Dann genauso bedienen wie auf dem PC.
  Auf dem Handy erscheint die Liste oben, die Auswahl unten.


════════════════════════════════════════════════════════════
  FILTER IN DER LISTE
════════════════════════════════════════════════════════════

  ALLE             → Alle Personen
  BAND             → Nur Bandnamen (Event-Titel)
  CREW             → Nur Technik-Personal
  STAGEMANAGER     → Nur Stagemanager
  KAMERA           → Alle Kamera-Rollen
  TON STREAM       → Streamton-Techniker
  TON FOH          → FOH-Tontechniker
  LICHT            → Lichttechniker
  SCHNITT          → Schnitttechniker
  PRODUKTION       → Produzenten
  VEREINSMITGLIED  → Vereinsmitglieder
  VORSTANDSMITGLIED→ Vorstandsmitglieder

  ▼ Alle Rollen → Weitere Rollen ausklappen
    (Instrumente, etc.)


════════════════════════════════════════════════════════════
  WAS ERSCHEINT IM LOWER THIRD?
════════════════════════════════════════════════════════════

  f0 (oben, groß)   = Name der Person / Band
  f1 (unten, klein) = Genre oder Rolle

  Beispiele:
    HIPHOP GIRLS RECKLINGHAUSEN  /  Tanz
    JULIAN                       /  Stagemanager
    ABANDONED HEAVEN             /  Rock
    SINA                         /  Kamera
    MAX MUSTERMANN               /  Vereinsmitglied

  Band ohne Genre → zeigt "Band"
  Crew            → zeigt die Rolle


════════════════════════════════════════════════════════════
  IP-ADRESSE ÄNDERN (neuer PC oder neues Netz)
════════════════════════════════════════════════════════════

  Seite öffnen → unten rechts: IP-Feld
  Neue IP eingeben → Enter oder ↺ klicken
  Wird automatisch gespeichert (auch nach F5)

  OnTime-PC-IP herausfinden:
  → Windows: cmd → ipconfig → "IPv4-Adresse"


════════════════════════════════════════════════════════════
  PASSWORT ÄNDERN
════════════════════════════════════════════════════════════

  Datei: AppData\Roaming\ontime\external\mm\index.html

  Suchen:   const PW = '1989';
  Ändern:   const PW = 'neuesPasswort';


════════════════════════════════════════════════════════════
  FEHLERBEHEBUNG
════════════════════════════════════════════════════════════

  Seite lädt nicht
  → OnTime gestartet? IP korrekt?
  → Handy: im gleichen WLAN wie der OnTime-PC?

  Passwort funktioniert nicht
  → Passwort ist: 1989 — F5 und nochmal

  Konzertname zeigt "Lade..." oder "OnTime"
  → OnTime → Settings → Project data → Project title prüfen

  Lower Third zeigt "Bandname / Genre"
  → Reihenfolge: ERST senden → DANN Play in Caspar!

  Genre wird nicht angezeigt
  → Feldname in OnTime muss "Gernre" heißen (Tippfehler!)
  → Kein Genre → zeigt automatisch "Band"

  OFFLINE-Screen erscheint
  → OnTime starten, dann F5

  Caspar zeigt Template nicht
  → CasparCG Server + Client neu starten

  Beim Band-Filter kommen Bandmitglieder
  → In index.html prüfen:
     if (activeRoleFilter === 'band') return t.isBandTitle === true;


════════════════════════════════════════════════════════════
  DATEI-ÜBERSICHT (Setup-Ordner)
════════════════════════════════════════════════════════════

  mm\
    index.html                   → Browser / Handy (OnTime-Seite)

  template\
    Lower thrid.html             → CasparCG Template
    scripts\gsap.min.js          → Animation
    media\*.ttf                  → Schrift
    media\*.svg                  → Logo / Grafik

  ANLEITUNG.txt                  → diese Datei

════════════════════════════════════════════════════════════
