# IRON — Marketing-Plan (laufend)

Gehört der Marketing-Baustelle (`feat/marketing`). Jede „Marketing-Runde"
hängt oben eine neue Runde an; ältere Runden bleiben darunter stehen, damit
der Rückblick etwas hat, woran er messen kann.

**Grenzen (gelten in jeder Runde):** Alles hier ist Entwurf. Nichts wird
gepostet, verschickt, gekauft oder angelegt ohne ausdrückliches Ja des
Nutzers. Braucht Marketing etwas in der App, steht es unten unter
„Für den Integrator".

**Auto-Zählen an der Uhr:** wird NICHT beworben, solange es nicht im Studio
bewiesen ist (`docs/watch-app.md`, Stufe B). Entwürfe dafür liegen nur in der
Schublade (Abschnitt S).

---

## Runde 1 — 02.10.2026

### Nachtrag: Antworten des Nutzers (02.10.)

- **Instagram und TikTok gibt es schon.** TikTok wird über Higgsfield
  verbunden (Freigabe-Link an den Nutzer, 02.10.). Für Instagram gibt es
  hier keinen Anschluss, also bleibt es bei fertigen Entwürfen zum
  Selbst-Posten. Gepostet wird weiterhin nur nach Ja pro Beitrag.
- **Freundestest über TestFlight statt Web.** So bekommen die Tester die
  iPhone-App mit Mitteilungen, Sperrbildschirm und Uhr. Ablauf siehe E1.
- **Vergleichs-Screenshot aus der App heraus statt von Hand.** Wird als
  Wunsch an den Integrator weitergegeben (I-6, Teilen-Bild aus dem echten
  Training). Damit bekommt auch jeder Nutzer ein teilbares Bild.
- **Gründerpreis: ja**, verbunden mit einem nummerierten Dankeschön-Abzeichen
  für die Ersten (Konzept „Die ersten 100" in 3c).

### Nachtrag 07.10.: IRON-Sticker (Nutzer-Wunsch; „Das Gewicht steht schon drin" auf Wunsch raus, vier lustige neu: 12 Beintag? Ich hab Termine · 13 Mein Plan: heben. Mein Kopf: Pizza. · 14 Ich komm nur wegen der Pause. · 15 Noch ein Satz. Sagt jeder. Schafft keiner.)

Vorschau mit elf Motiven: https://claude.ai/artifact/LSMCsZ8VjynKcaU32ijLcJ
(privat, nur für den Nutzer). Druckdateien erst nach Auswahl.

| Nr. | Spruch | Form | Status |
|---|---|---|---|
| 01 | Das war der letzte Satz. (Lüge.) | Hantelscheibe Ø 6 cm | jetzt |
| 02 | Satz-Zeile „82,5 kg · IRON schlägt vor" | 9 × 3,7 cm | Zahl aus echtem Training (E-10) |
| 03 | Du hebst. IRON rechnet. | 7 × 4,2 cm | jetzt, Favorit |
| 04 | Pause: 1:30. Nicht 9 Minuten. | Timer Ø 6 cm | jetzt |
| 05 | Hantel zurück. Dein Nachfolger dankt. | 8 × 5,2 cm | nur mit Erlaubnis des Studios |
| 06 | Nicht entscheiden. Trainieren. | Pille 8 × 4,4 cm | jetzt |
| 07 | +2,5 kg. Jede Woche ein bisschen. | 5 × 5 cm | jetzt |
| 08 | Handy bleibt in der Tasche. | 7 × 4,2 cm | ab TestFlight/Store |
| 09 | App-Symbol | 4 × 4 cm | jetzt |
| 10 | Gründer · Nr. ___ | Ø 6 cm, Gold | zu „Die ersten 100" |
| 11 | Scannen. Training, das mitdenkt. + QR | 8 × 5,2 cm | später, braucht I-8 |

Regeln: Vinyl matt, erste Auflage 3–4 Motive je 25–50 Stück (grob 30–60 €,
Angebot holen, nichts bestellt). Nur auf eigene Sachen, an Tester, im Studio
nur mit Erlaubnis — nie wild kleben.

### 1. Lage: was ist neu, was ist erzählenswert

Seit der Strategie vom 08.09. hat sich der Rahmen verschoben. Mehrere Sätze
in `marketing-strategie.md` gelten nicht mehr:

| Damals (08.09.) | Heute (02.10.) |
|---|---|
| Kein App Store bis Dezember | iPhone-App läuft (über Xcode), App Store Connect, RevenueCat und TestFlight stehen beim Nutzer auf der Liste |
| Keine Webseite | Eigener Webseiten-Chat (`~/iron-web`) seit 01.10. |
| Keine Domain | `ironhq.de` gekauft, Mail-Absender läuft darüber |
| Link-Vorschau leer (A1) | **erledigt**: Titel, Text, Bild 1200×630 in `index.html` |
| Preis fest 4,99 / 39,99 | Preis kommt aus dem Store; Gründerpreis und Probeabo geplant (`plan-preise.md`) |

Neu in der App und erzählenswert (nach `bereichskarte.md`):

| Neu | Taugt als Story? | Wann |
|---|---|---|
| **Ganzes Training am Sperrbildschirm** (Live Activity, Gewicht ±, 23.09.) | Ja — das stärkste neue Bild: „Handy bleibt in der Tasche." Zeigt, dass IRON fürs Studio gebaut ist. | Erst wenn die iPhone-App für Fremde installierbar ist (Store/TestFlight). Im Web gibt es das nicht. |
| Apple-Watch-App, Pausenton bei gesperrtem Handy | Ja, als Beleg zum Sperrbildschirm | wie oben |
| Coach-Chronik („weiß ich seit …") | Ja, der emotionale Spot — braucht Wochen echter Daten | jetzt sammeln, später zeigen |
| „Deine Sprüche" | klein, nett für Bestandsnutzer | nicht nach außen |
| Anmeldung per Code (Mail von `ironhq.de`) | kein Werbethema, aber nimmt eine Hürde weg | — |
| **Auto-Zählen (IRON+)** | sehr stark — **noch nicht bewerben** | nach Studio-Test, siehe Abschnitt S |
| Vorausgefülltes Gewicht | bleibt die Kernbotschaft | jetzt |

### 2. Zahlen (Supabase, nur Summen, nur gelesen)

| Messung | Wert |
|---|---|
| Konten gesamt | 5 |
| Neue Konten letzte 14 Tage | 0 |
| Konten, die je ein Training hochgeladen haben | 1 |
| Aktiv letzte 7 / 28 Tage (mit Konto) | 1 / 1 |
| Noch dabei 21 Tage nach Anmeldung | 1 von 5 |
| Trainings gesamt / letzte 14 Tage | 24 / 15 |
| IRON+ bezahlt / Zahlungen | 0 / 0 |
| Testmonat gestartet | 1 |
| Einladungscodes / eingelöst | 1 / 0 |
| Feedback gesamt / letzte 14 Tage | 13 / 3 |
| Geräte (`device_pings`) gesamt / neu in 14 Tagen | 34 / 32 |

**Was das heißt:** Außer einer Person (vermutlich der Nutzer selbst)
trainiert niemand sichtbar mit IRON. Die 32 „neuen Geräte" passen nicht zu 0
neuen Konten. Wahrscheinlich sind das Test-Browser der Chats und der
Simulator. Das ist eine Vermutung, gemessen ist es nicht.

**Was fehlt, damit Zahlen etwas sagen:**
1. Test-Geräte von echten trennen (siehe I-2).
2. Woher jemand kommt: WhatsApp, Forum, Store (I-3).
3. Wer ohne Konto trainiert, ist für uns unsichtbar (local-first, gewollt).
   Gezählt werden darf nur die Zahl, nie der Inhalt: „Gerät hat diese Woche
   trainiert: ja/nein" am `device_ping` (I-2).

### 3. Plan 02.10.–16.10.

Ziel der zwei Wochen: **die ersten 5 echten Menschen außer dir**, die zwei
Wochen lang mit IRON trainieren. Noch keine Reichweite. Die Zahlen oben
zeigen, dass vorher niemand drin ist, dessen Verhalten wir lernen können.

#### 3a. Social Media / Nachrichten — fertige Texte

**Beitrag 1 — WhatsApp an 5 Freunde, die schon trainieren (Kanal: persönlich, du selbst)**
Bild: keins, der Link bringt die Vorschau mit (A1 ist erledigt).

> Hey, ich hab in den letzten Monaten eine Trainings-App gebaut: IRON. Sie
> trägt dir das Gewicht für jeden Satz schon ein — aus dem, was du letztes
> Mal geschafft hast. Hast du Lust auf einen Test? 2 Wochen dein normales
> Training, nichts extra. Ich frag dich nur einmal pro Woche eine Sache.
> Mit meinem Code bekommen wir beide 14 Tage IRON+: [Einladungslink aus der App]

Woche 1 nachfragen: *„Hat IRON dir ein Gewicht vorgeschlagen, das nicht
gepasst hat? Welches?"* · Woche 2: *„Was hast du gesucht und nicht gefunden?"*

**Beitrag 2 — WhatsApp-Status / Instagram-Story (privates Konto, Kanal: du selbst, ohne Gesicht)**
Bild: Bildschirmfoto der Satz-Tabelle aus deinem echten letzten Training,
vorausgefülltes Gewicht sichtbar, darüber in Weiß:

> Ich hab nichts eingetippt. Die Zahl stand schon da.

Darunter der Link. Keine erfundenen Zahlen (E-10).

**Beitrag 3 — Antwort-Vorlage für Forum/Reddit (erst NACH den vier Wochen Mitlesen, Strategie §6)**
Für Threads der Art „Welche Tracker-App nutzt ihr?":

> Ich nutze/teste gerade drei: [App A] für X, [App B] für Y, und IRON — die
> ist von mir, noch früh und gerade kostenlos. Unterschied: Das Gewicht für
> jeden Satz steht schon drin, aus deinem letzten Training gerechnet. Wenn
> jemand testen mag, freu ich mich über ehrliche Kritik: [Link]

Diese Runde: **nur 2–3 deutschsprachige Kraftsport-Gruppen aussuchen und mitlesen**,
nichts posten. Die Liste schreibe ich in der nächsten Runde, wenn du sagst,
wo du ohnehin liest.

**Entscheidung nötig: eigener Insta/TikTok-Kanal?**
Die Strategie sagt nein (zu wenig Zeit, kein Gesicht). Du wünschst dir jetzt
ausdrücklich Social Media. Mein Vorschlag als Mittelweg: **Namen sichern
(@iron… auf Instagram und TikTok), ein Profilbild, Link, sonst nichts.**
Echte Beiträge erst, wenn die iPhone-App installierbar ist. Dann gibt es
mit dem Sperrbildschirm-Training ein Video, das sich ohne Gesicht erzählt.
Anlegen nur nach deinem Ja.

Vorbereitet für diesen Tag (Reel, 9:16, 8–12 s, Bildschirmaufnahme + Studio-B-Roll ohne Gesicht):
> Text im Bild: „Handy in der Tasche. Training läuft trotzdem." —
> Sperrbildschirm zeigt nächsten Satz, Daumen tippt ✓, Pause läuft.
> Schluss: „IRON — Training, das mitdenkt."

#### 3b. Store-Texte / -Bilder

- `marketing-appstore.md` ist inhaltlich gut, aber zwei Dinge sind veraltet:
  die Begründung „erst Web" und der feste Preis im Text. Preis im Store-Text
  erst eintragen, wenn er in App Store Connect steht (er kommt aus dem Store).
- **Bild 1** bleibt der Vergleich „leeres Feld gegen eingetragene Zahl".
  **Neu als Bild 3: Sperrbildschirm mit laufendem Training.** Das hatte
  damals noch keine andere App in der Reihe, und es ist ein echtes iPhone-Feature.
- **Fehlt weiter:** der Vergleichs-Screenshot aus einem echten Training.
  Ohne ihn gibt es weder Store-Bild 1 noch Beitrag 2 in voller Stärke.
  Das braucht eine Stunde von dir (Strategie §6).

#### 3c. Verkauf

- **Jetzt nichts verkaufen.** 0 zahlende Abos sind in dieser Phase richtig
  (Strategie §9). Erst Leute, die bleiben.
- **Gründerpreis (PR-2) — mein Vorschlag zu deinen drei offenen Fragen:**
  1. Bis wann: **festes Datum**, 8 Wochen nach dem Store-Start. Ehrlicher als
     „erste N Käufer" und braucht keinen Server-Zähler.
  2. Höhe: rund **40 % unter Normalpreis** (bei 4,99/39,99 also etwa
     2,99 € / 24,99 €). Der Betrag steht nur im Store.
  3. Gründer **behalten den Preis** bei späteren Erhöhungen (PR-1). Das ist
     das eigentliche Versprechen und kostet heute nichts.
- **Konzept „Die ersten 100" (Nutzer-Idee 02.10., ausgearbeitet):**
  - Wer zu den ersten 100 Konten nach Store-Start gehört, bekommt ein
    **nummeriertes Abzeichen**, z. B. „Gründer · Nr. 37". Es ist kostenlos
    und bleibt für immer sichtbar: im Profil, neben dem Namen in der
    Rangliste und bei Freunden. Eine Nummer ist mehr wert als ein Häkchen,
    weil jede nur einmal vergeben wird.
  - **Dieselben 100 haben Anrecht auf den Gründerpreis**, solange das
    Fenster offen ist (8 Wochen). Wer kauft, behält ihn dauerhaft.
  - Nach Nr. 100 ist Schluss. Die Seite zeigt ehrlich „noch 23 Plätze".
    Das ist kein Countdown-Druck, sondern ein echter Zähler.
  - **Warum 100 und nicht 1000:** Bei heute 5 Konten sieht „17 von 1000"
    leer aus, „17 von 100" fühlt sich exklusiv an. Ist die Liste schnell
    voll, kann eine zweite Welle folgen („Die ersten 1000", ohne Preis,
    nur Abzeichen).
  - **Nicht „Club" nennen:** In der App gibt es schon den „100er Club" für
    100 kg Gewicht (`milestones.ts`, `achievements.ts`). Das würde
    verwechselt. Vorschlag: **„Gründer"** oder **„Die ersten 100"**.
  - Die TestFlight-Tester aus E1 bekommen automatisch die Nummern 1–5.
    Das ist auch ein gutes Argument, beim Test mitzumachen.
- Botschaft dazu (fertig, ohne Druck):
  > Du bist früh dabei. Dafür zahlst du weniger — solange du bleibst.
- **Probeabo über Apple (PR-4)** senkt die Anmeldungen, bringt aber echte
  Abos. Für die „ersten 5"-Phase spielt es keine Rolle, weil Freunde über
  den Einladungscode kommen.

#### 3d. Partnerschaften / Influencer

Bleibt in der Schublade (`marketing-influencer.md` §4). Keine der
Bedingungen ist erfüllt: Wir wissen nicht, wie lange jemand bleibt (1 von 5).
**Ein kostenloser Schritt jetzt:** Frag dein eigenes Studio, ob du einen
Zettel mit QR-Code ans Schwarze Brett hängen darfst. Den Entwurf schreibe
ich auf Zuruf (A5-Format, QR auf den Einladungslink).

#### 3e. Experiment dieser Runde

**E1 — Fünf-Freunde-Test über TestFlight** (geändert 02.10.).
- Was: Beitrag 1 an genau 5 Leute, die schon trainieren. **Mindestens
  einer mit Apple Watch.** Der kann nebenbei Auto-Zählen Stufe B aufnehmen
  (`watch-app.md`), damit wird später das stärkste Werbethema frei.
- Voraussetzungen, alle beim Nutzer: bezahlter Apple-Developer-Account,
  App „IRON" in App Store Connect, in Xcode *Product → Archive →
  Distribute → TestFlight* hochladen (die Uhr-App reist im selben Build
  mit). Dann **externe Tester mit öffentlichem Link** anlegen. Für den
  ersten Build prüft Apple kurz (Beta-Review, meist etwa ein Tag). Interne
  Tester bräuchten Zugang zu deinem App-Store-Connect-Team, das passt für
  Freunde nicht. Ein Build läuft nach 90 Tagen ab.
- Achtung Mitteilungen: Erinnerungen und Pausenton kommen vom Gerät selbst
  und funktionieren. Sofort-Push vom Server (z. B. Anfeuern) erreicht die
  iPhone-App laut `stand.md` (17.09.) noch nicht. Das ist kein Hindernis
  für den Test, aber man sollte es wissen.
- Nachricht (ersetzt Beitrag 1):
  > Hey, ich hab eine Trainings-App gebaut: IRON. Sie trägt dir das Gewicht
  > für jeden Satz schon ein — aus dem, was du letztes Mal geschafft hast,
  > auch auf der Apple Watch. Magst du 2 Wochen testen? Dein normales
  > Training, ich frag nur einmal pro Woche eine Sache. Du bekommst dafür
  > eine der ersten Gründer-Nummern.
  > 1. „TestFlight" aus dem App Store laden  2. diesen Link öffnen: [TestFlight-Link]
- Messgröße (aus Supabase, nur Summen): **eingelöste Codes** (heute 0) und
  **Konten mit ≥ 3 Trainings in 14 Tagen** (heute 1).
- Ziel bis 16.10.: 3 Codes eingelöst, 2 Leute mit ≥ 3 Trainings.
- Gelernt wird so oder so: Unter 3 eingelösten Codes liegt es an der Nachricht
  oder am Einstieg. Dann frage ich nach, wo sie hängen geblieben sind.

### 4. Rückblick (auf den Plan vom 08.09.)

| Vorhaben | Lief? |
|---|---|
| A1 Link-Vorschau | ✅ gebaut. **Ungeprüft:** Link einmal per WhatsApp an dich selbst schicken und nachsehen, ob Bild + Text kommen |
| A2 Hinweis „auf den Startbildschirm legen" | ❓ im Code nicht gefunden. Wird mit der Store-App unwichtiger |
| A3 Preis/Konto im Einstieg | teilweise: Die Vorschau sagt „Kostenlos starten, kein Konto nötig" |
| Vergleichs-Screenshot | ❌ nicht vorhanden |
| Fünf Freunde, vier Wochen | ❌ nicht gelaufen (0 neue Konten, 1 aktiv) |
| Foren mitlesen | ❌ nicht begonnen |

**Was wir lernen:** Die Zeit ist komplett ins Produkt geflossen. Das war
richtig, weil die App jetzt stabil ist (0 Befund-Marker). Aber nach drei
Wochen hat noch kein Fremder trainiert. Deshalb hat ab jetzt **ein Mensch
von außen** Vorrang vor jeder weiteren Funktion. Die Strategie bekommt
einen Hinweis, dass ihr Rahmen (kein Store, keine Webseite) überholt ist.

### 5. Nächste Schritte (nach Wirkung)

1. **TestFlight aufsetzen und 5 Tester einladen, einer davon mit Apple Watch** (E1, Nachricht steht fertig).
2. **Teilen-Bild aus der App** als Wunsch beim Integrator (I-6), statt es von Hand zu machen.
3. **Link-Vorschau prüfen:** App-Link per WhatsApp an dich selbst schicken. 1 Min.
4. ✅ Gründerpreis entschieden, mit „Die ersten 100" (I-7).
5. ✅ Konten sind da. TikTok über Higgsfield verbinden (Link bestätigen).

---

## Für den Integrator

Übergaben aus Runde 1. Keine Aufträge an andere Chats, nur Hinweise.
Zuordnung entscheidet der Integrator.

- **I-1 Bewertungs-Teilen zeigt auf eine andere Adresse.**
  `src/components/RatingPrompt.tsx:5` teilt `https://iron-tracker.pages.dev`,
  alle anderen Stellen nutzen `https://iron-gym-tracker.vercel.app`
  (`referral.ts`, `authCallback.ts`, `index.html`). Wer nach dem Bewerten
  teilt, schickt wahrscheinlich einen toten oder falschen Link. Erreichbarkeit
  konnte ich aus der Cloud nicht prüfen (Netz gesperrt). Bitte prüfen und
  auf die eine App-Adresse stellen.
- **I-2 Echte Geräte zählbar machen.** `device_pings`: 34 Geräte, davon 32
  neu in 14 Tagen, bei 0 neuen Konten. Bitte Test-Umgebungen nicht pingen
  oder markieren (localhost, Vercel-Vorschau, `navigator.webdriver`,
  Simulator). Wenn möglich zusätzlich ein Feld „hat diese Woche trainiert"
  (ja/nein, kein Inhalt). Nur so sehen wir Nutzer ohne Konto.
- **I-3 Herkunft messen.** `?src=whatsapp|forum|qr|store` beim ersten Öffnen
  merken und einmal mit dem Geräte-Ping mitschicken, nur den Kanalnamen.
  Muster wie `capturePendingRef()` in `referral.ts`. Ohne das wissen wir nach
  dem ersten Forum-Beitrag nicht, ob er gewirkt hat.
- **I-4 Adresse bei Umzug auf `ironhq.de`.** Falls die Web-App dorthin zieht:
  `og:url`/`og:image` (`index.html`), `APP_URL` (`referral.ts`),
  `CANONICAL_APP_URL` (`authCallback.ts`), Gegenstück in `store.tsx` und I-1
  gemeinsam umstellen. Danach Vorschau-Cache beachten.
- **I-5 Status A2/A4 aus `stand.md` (08.09.) klären:** Hinweis „auf den
  Startbildschirm legen" im Code nicht gefunden. Teilen nach neuem Rekord
  (A4) ebenfalls nicht. Erledigt, verworfen oder offen?

- **I-6 Vergleichs-/Teilen-Bild aus der App** (Nutzer-Wunsch 02.10.).
  Ein Knopf am Trainingsende („Teilen") erzeugt ein Bild aus dem echten
  Training: Satz-Tabelle mit der Zahl, die IRON vorgeschlagen hat, Marker
  „IRON schlägt vor", darunter „Ich hab nichts eingetippt." und die
  App-Adresse. Echte Zahlen, nichts erfunden (E-10). Damit hat Marketing
  sein Bild 1 und jeder Nutzer etwas zum Teilen. Ähnliches Muster gibt es
  schon mit der Sieger-Bildkarte (`WinnerCardSheet.tsx`, laut `stand.md`
  ungenutzt).
- **I-7 „Die ersten 100" (Gründer-Abzeichen + Gründerpreis)**, Konzept in
  3c. Braucht eine fortlaufende Nummer vom Server je Konto (erste 100 nach
  Store-Start, TestFlight-Tester zuerst), ein Abzeichen in Profil/Rangliste
  und die Freischaltung des Gründer-Angebots (`plan-preise.md` PR-2, eigenes
  RevenueCat-Offering) nur für diese Konten. Name nicht „Club" (Verwechslung
  mit dem 100-kg-Club).

- **I-8 Kurz-Adresse für QR-Codes (Sticker, Aushang).** `ironhq.de/s`
  (oder ähnlich) leitet auf die App weiter und hängt `?src=sticker` an.
  Gedruckte QR-Codes zeigen nie direkt auf `vercel.app`, damit sie gültig
  bleiben, wenn das Ziel wechselt (Web → App Store). Zählen setzt I-3
  voraus. Die Domain liegt beim Webseiten-Chat bzw. Nutzer.

---

## S. Schublade — vorbereitet, NICHT verwenden

**Auto-Zählen an der Uhr.** Freigabe erst, wenn Stufe B im Studio bestanden
ist und eine Trefferquote vorliegt (`watch-app.md`). Dann auch erst PR-1.

- Kernsatz: *„Trainiere einfach. IRON zählt."*
- Reel (9:16, 10 s): Hand mit Uhr curlt, auf der Uhr läuft die Zahl mit
  3 … 4 … 5, Hantel ab, Uhr: „Stimmt die Zahl? 8" → Krone → ✓. Text: *„Du
  hebst. Die Uhr zählt. Du drückst nur noch ✓."*
- Ehrlichkeits-Regel: Nennen, für welche Übungen es geht (anfangs nur Curls),
  und die echte Trefferquote. Nie „zählt alles".
- Entdecken-Karte (Entwurf): *Zählt mit, während du hebst* — die Uhr erkennt
  deine Wiederholungen bei Curls, du bestätigst nur → Training.
