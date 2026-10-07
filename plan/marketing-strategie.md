# IRON — Marketing-Strategie

Stand: 2026-09-08. Geschrieben für die nächsten zwölf Wochen, nicht für
"irgendwann". Diese Datei gehört der Marketing-Baustelle
(`/Users/josiias878/iron-marketing`, Branch `feat/marketing`).

Alles hier steht auf vier Antworten des Nutzers, nicht auf Annahmen:

| Frage | Antwort |
|---|---|
| Trittst du selbst öffentlich auf? | **Nein — nur die Marke IRON.** Kein Gesicht, kein Name. |
| Wie viel Geld pro Monat? | **Unter 100 €.** |
| Wie viel Zeit pro Woche? | **2 bis 5 Stunden.** |
| Was soll in drei Monaten herauskommen? | **Erste echte Nutzer und Feedback.** Nicht Umsatz, nicht Reichweite. |
| App Store? | **Noch gar nichts** — kein Entwicklerkonto, kein Eintrag. |
| Wer würde die App heute benutzen? | **Eine Handvoll Freunde.** |

Wenn sich eine dieser Antworten ändert, ist die halbe Strategie hinfällig.
Dann diese Datei neu aufmachen, nicht drumherum arbeiten.

> **Hinweis 02.10.2026:** Zwei Antworten haben sich geändert. Der App Store
> wird vorbereitet (TestFlight, App Store Connect), und es gibt einen
> Webseiten-Chat samt Domain `ironhq.de`. A1 (Link-Vorschau) ist erledigt.
> Was daraus folgt, steht laufend in `docs/marketing-plan.md`. Eine
> Neufassung dieser Datei kommt, sobald der Store-Termin feststeht.

---

## 1. Die Lage, ohne Schönfärberei

Rechne selbst nach: 12 Wochen mal 3,5 Stunden sind rund **42 Stunden
Marketing insgesamt**. Das ist eine Arbeitswoche. Damit kann man genau
drei Dinge richtig machen — oder fünfzehn Dinge halb.

Und das Budget: unter 100 € im Monat. Das Apple-Entwicklerkonto allein
kostet rund 99 € im Jahr. Jede Strategie, die Geld voraussetzt, ist hier
keine Strategie, sondern ein Wunsch.

Daraus folgt eine unbequeme Regel, die im ganzen Dokument gilt:

> **Was Geld oder Dauerpflege kostet, fliegt raus. Was das Produkt selbst
> erledigt, bleibt.**

## 2. Der Befund, der alles andere aufhält

*Korrektur vom 2026-09-08: Hier stand zuerst, die Adresse werfe Fremde ohne
jede Erklärung in die App. Das war falsch. Ich hatte den Willkommens-Screen
mitten im Bildwechsel erwischt — Bilder noch nicht geladen, Text halb
eingeblendet — und aus einem einzigen Standbild geschlossen, es gäbe keinen
Text. Der Nutzer hat widersprochen, ich habe nachgesehen. Genau davor warnt
`design-language.md`: "mehr als einmal war der vermutete Bug in Wahrheit ein
Messfehler."*

**Der Willkommens-Screen ist gut.** Drei Karten, jede mit einer echten
Aufnahme aus der App: der fertige Tagesplan mit fünf Übungen ("Dein Plan
steht schon"), das Mitdenken, die Körper-Übersicht ("Dein Körper zeigt, was
fehlt"). Dazu ein erklärender Satz je Karte und darunter die Zusammenfassung
"1 Entscheidung — den Rest übernimmt IRON." Wer dort ankommt, versteht
innerhalb von zehn Sekunden, worum es geht.

Das Problem liegt eine Ebene davor: **die meisten Menschen kommen dort nie
an.**

`index.html` enthält im Kopf genau eine einzige Angabe über IRON:
`<title>IRON</title>`. Keine Beschreibung, kein Vorschaubild, nichts.

Was das heißt: Jeder geteilte Link — WhatsApp, Instagram-Nachricht, Discord,
Forum — erzeugt **ein leeres graues Kästchen mit dem Wort "IRON"**. Kein
Bild, kein Satz, kein Hinweis, worum es geht. In einem Chatverlauf, in dem
jeder andere Link ein Bild und zwei Zeilen Text mitbringt, sieht das aus wie
ein kaputter oder unseriöser Link. Die meisten tippen gar nicht erst darauf.

Und es trifft ausgerechnet die beiden Werkzeuge, die längst gebaut und
bezahlt sind:

- **Das Empfehlungsprogramm.** `shareInvite()` in `src/lib/referral.ts`
  verschickt genau so einen Link — das ist der ganze Zweck der Funktion.
  Jede Empfehlung, die ein Nutzer ausspricht, landet als graues Kästchen im
  Chat seines Freundes.
- **Die Sieger-Bildkarte.** Sie trägt die App-Adresse unten drauf, laut
  `docs/stand.md` ausdrücklich als "der Rückweg zu uns — ohne den verpufft
  die ganze Umkehr-Idee". Der Rückweg endet beim selben grauen Kästchen.

Der gesamte Wachstumsplan hängt an geteilten Links. Solange die Vorschau
leer ist, ist es gleichgültig, wie gut der Bildschirm dahinter aussieht —
niemand kommt bis dorthin. Deshalb ist die Link-Vorschau **Vorhaben Nummer
eins** (Anforderung A1). Der Integrator repariert sie.

Ein zweiter, leiserer Verlust bleibt daneben bestehen: Auf dem iPhone ist
IRON nur dann eine richtige App, wenn man sie über den Teilen-Knopf **auf
den Startbildschirm legt**. Das weiß kein normaler Mensch. Ohne diesen
Hinweis bleibt IRON für viele "eine Website, die ich mal aufhatte", und ist
am nächsten Tag vergessen (Anforderung A2).

Und ein dritter, der beim Nachsehen auffiel: **Nirgends steht, was IRON
kostet und ob man ein Konto braucht.** Das sind die zwei Fragen, die jeder
Fremde stellt, bevor er irgendetwas antippt. Wer sie nicht beantwortet
findet, vermutet das Schlechtere — dass beides gleich kommt und unangenehm
wird (Anforderung A3).

### Keine eigene Werbe-Startseite

Entscheidung des Nutzers vom 2026-09-08: Es wird **keine** separate
Werbeseite gebaut. **Die App ist die Demo.** Der Willkommens-Screen leistet
bereits, wofür man sonst eine Landingpage bauen würde, und er tut es mit
echten Aufnahmen statt mit Versprechen.

Das ist die richtige Entscheidung, und sie spart genau die Sorte Arbeit, die
sich ein Einzelkämpfer nicht leisten kann. Was fehlt, ist nicht eine neue
Seite — es sind fünf Zeilen im Kopf einer Datei, die es schon gibt.

## 3. Was IRON ist — in einem Bild, nicht in einem Satz

Der Untertitel "TRAINING, DAS MITDENKT" ist gut, aber er ist eine
Behauptung. Behauptungen glaubt niemand; Fitness-Apps behaupten alle etwas.

Der Unterschied von IRON lässt sich **zeigen**, und zwar in einem einzigen
Bild:

> Zwei Bildschirme nebeneinander. Links irgendeine andere Tracker-App:
> Bankdrücken, Satz 1, **ein leeres Feld**. Rechts IRON: Bankdrücken,
> Satz 1, **42,5 kg — schon eingetragen**, daneben der Marker
> "IRON schlägt vor".
>
> Darunter ein Satz: *"Der eine hat dich gefragt. Der andere hat sich
> gemerkt, was du letzte Woche gehoben hast."*

Das ist die vollständige Werbebotschaft. Kein Video, kein Gesicht, kein
Geld, keine Musik. Ein Bild, das man überall hinposten kann, wo jemand nach
einer Tracker-App fragt. Für eine gesichtslose Marke mit 42 Stunden
Gesamtbudget ist das die einzige Werbung, die trägt.

Der Nutzer hat diesen Gedanken selbst schon gehabt — er steht als Befund in
`docs/stand.md` ("der Satz-Tabellen-Ausschnitt mit bereits eingetragenem
Gewicht"). Er wurde dort für den Willkommens-Screen notiert. Er ist aber
mehr als das: **er ist die Positionierung.** Derselbe Ausschnitt gehört auf
die Link-Vorschau, in jeden Forenbeitrag, später auf das erste
App-Store-Bild.

Eine Sache noch, und die ist wichtig: Dieses Bild darf **nie gestellt sein**.
Kein erfundenes Gewicht, keine Fantasie-Kurve. Die Zahl auf dem Screenshot
muss aus einem echten Training kommen. `docs/design-language.md` sagt für
die App: "Sie behauptet nichts, was sie nicht weiß. Vertrauen ist hier das
Produkt." Das gilt für die Werbung genauso — sonst verkaufst du etwas
anderes, als du gebaut hast, und merkst es erst an den Ein-Stern-Bewertungen.

## 4. Wen wir zuerst holen

Auf die Frage nach der Zielgruppe kam: *"Es gilt definitiv für Anfänger und
für Fortgeschrittene. Natürlich wäre es super, wenn man die Konkurrenz
übertrumpft und von denen Kunden bekommt."*

Der zweite Satz ist die bessere Antwort als der erste — und er ist deine
eigene.

**Wir holen die Umsteiger.** Menschen, die heute schon Hevy, Strong oder
Ähnliches benutzen und dort in leere Felder tippen. Vier Gründe, und keiner
davon ist Geschmackssache:

1. **Man findet sie.** Sie reden in Foren, sie bewerten Apps, sie fragen
   öffentlich nach Alternativen. Anfänger fragen nicht — sie wissen noch
   nicht, dass sie ein Problem haben.
2. **Sie verstehen das Bild aus Abschnitt 3 sofort.** Man muss ihnen nichts
   erklären. Sie haben genau dieses leere Feld letzten Dienstag angestarrt.
3. **Sie benutzen die App wirklich.** Sie tracken schon, das ist Gewohnheit.
   Genau davon hängt dein Ziel ab: Feedback bekommt man nur von Leuten, die
   die App vier Wochen lang benutzen — nicht von Leuten, die sie anschauen.
4. **Ihr Feedback taugt etwas.** Ein Anfänger sagt "ganz cool". Ein
   Umsteiger sagt "der Vorschlag nach einer Woche Pause war Quatsch, ich
   hatte Grippe". Der zweite Satz macht die App besser.

**Anfänger sind damit nicht abgeschrieben** — im Gegenteil, sie sind später
die größere Gruppe. Aber sie sind nicht die *ersten*. Sie brechen häufiger
ab, sie können nicht sagen, was fehlt, und sie kommen ohnehin von selbst,
sobald die App eine Weile existiert und empfohlen wird.

Und die Botschaft trägt am Ende beide, weil sie unter beiden Nöten dieselbe
ist:

- Anfänger: *"Ich weiß nicht, welches Gewicht ich nehmen soll."*
- Fortgeschrittene: *"Ich weiß es schon — ich habe nur keine Lust, es jedes
  Mal selbst auszurechnen und mir zu merken."*
- IRON, für beide: **"Du musst nicht entscheiden."**

Das ist der Satz hinter dem Untertitel. Er steht in keiner Werbung, er ist
der Prüfstein: Wenn eine Marketing-Idee diesen Satz nicht stützt, gehört sie
nicht dazu.

## 5. MCI: nicht antreten, sondern danebenstellen

MCI von Tim Gabel wurde von über 30 Leuten gebaut — Sportwissenschaftler,
Ärzte, Programmierer —, mit einer siebenstelligen Investition und rund 20
Monaten Entwicklung. Es macht Kraft, Ernährung, Cardio, Beweglichkeit und
erkennt per Kamera Haltungsfehler. Getragen wird es von der Reichweite einer
bekannten Person.

Dagegen gewinnst du auf keinem einzigen Feld. Nicht bei Funktionsumfang,
nicht bei Budget, nicht bei Bekanntheit. Wer versucht, "das bessere MCI" zu
sein, verliert jeden Vergleich, den er selbst eröffnet hat.

Aber der Vergleich ist auch der falsche. **MCI verkauft dir einen
Trainingsplan. IRON verkauft dir deine eigene Vergangenheit, klug
ausgewertet.** Bei MCI kommt die Vorgabe von außen — von deren Team, deren
Wissenschaftlern, deren Programm. Bei IRON kommt sie aus dem, was *du*
letzte Woche tatsächlich gehoben hast.

Das ist kein kleineres MCI. Das ist die Gegenrichtung. Und es ist ein
Vorteil, den ein 30-Personen-Team nicht wegprogrammieren kann, weil er nicht
an Aufwand hängt, sondern an der Haltung.

Praktische Regel: **MCI nie namentlich in der Werbung erwähnen.** Wer einen
größeren Konkurrenten nennt, macht kostenlos Werbung für ihn und stellt sich
selbst als den kleineren daneben. Die Abgrenzung passiert über das Bild aus
Abschnitt 3 — gegen leere Felder, nicht gegen Namen.

## 6. Der Plan: zwölf Wochen, drei Vorhaben

Nicht mehr als drei. Bei 42 Stunden ist alles Weitere Selbstbetrug.

### Wochen 1–3: Die Vorschau reparieren lassen (ca. 4 Stunden)

Ohne die passiert alles andere umsonst. Zu tun:

- **Die Link-Vorschau anfordern** (A1) und die Texte dafür liefern — stehen
  fertig in Abschnitt 7. Gebaut wird sie vom Integrator, das sind wenige
  Zeilen in `index.html`.
- Den "auf den Startbildschirm legen"-Hinweis anfordern (A2), Preis- und
  Konto-Frage anfordern (A3).
- **Den Vergleichs-Screenshot bauen.** Aus einem echten Training. Das ist
  Handarbeit von dir, kein Auftrag an eine Baustelle: zwei Aufnahmen, eine
  aus einer anderen App, eine aus IRON, nebeneinandergelegt. Eine Stunde.
  Das Bild wird zwölf Wochen lang gebraucht — in Foren, im Chat, später im
  App Store.
- **Danach einmal selbst prüfen:** die Adresse an dich selbst per WhatsApp
  schicken und nachsehen, ob Bild und Text erscheinen. Nicht darauf
  verlassen, dass es gebaut wurde — nachsehen.

### Wochen 2–6: Die fünf Freunde — aber richtig (ca. 8 Stunden)

Fünf Freunde sind kein Notbehelf. Sie sind der ganze Test.

Nicht "probier mal aus" schicken. Sondern eine Verabredung:

> "Vier Wochen, dein normales Training, du trägst nichts extra ein. Ich
> frage dich einmal pro Woche eine einzige Frage."

Die eine Frage pro Woche, immer verschieden, immer konkret:
1. Woche: *"Hat IRON dir ein Gewicht vorgeschlagen, das falsch war? Welches?"*
2. Woche: *"Was hast du gesucht und nicht gefunden?"*
3. Woche: *"Hast du diese Woche ohne die App trainiert? Warum?"*
4. Woche: *"Würdest du 4,99 € dafür zahlen? Ehrliche Antwort, ich bin nicht
   beleidigt."*

Die vierte Woche ist die wichtigste. **Wer in Woche 3 noch trainiert, ist
der Beweis. Wer aufhört, ist die Information.** Frag jeden, der aufhört,
nach dem Grund — das ist die wertvollste Nachricht, die du in diesen zwölf
Wochen bekommst, wertvoller als zehn neue Anmeldungen.

Schreib die Antworten mit. Nicht im Kopf behalten.

### Wochen 5–12: Dorthin gehen, wo die Umsteiger reden (ca. 20 Stunden)

Für eine Marke ohne Gesicht gibt es genau einen kostenlosen Weg nach außen:
**Orte, an denen Text zählt statt Person.** Foren, Reddit, Facebook-Gruppen,
Discord-Server rund ums Krafttraining auf Deutsch.

Die Regel dabei ist unromantisch und wird meistens gebrochen:

> **Vier Wochen mitlesen und antworten, ohne IRON ein einziges Mal zu
> erwähnen.**

Wer in einer Gruppe als Erstes seine App verlinkt, ist ein Werbender und
wird entfernt. Wer vier Wochen lang hilfreiche Antworten gibt, ist ein
Mitglied — und darf danach sagen "ich baue selbst eine App, die genau das
macht, hier ist sie". Der Unterschied zwischen diesen beiden Wegen ist der
Unterschied zwischen null und den ersten dreißig Nutzern.

Konkret, pro Woche etwa 90 Minuten:
- 2–3 Gruppen aussuchen (nicht mehr), in denen wirklich über Training
  geredet wird und nicht nur Bilder gepostet werden.
- Auf Fragen antworten, bei denen du wirklich etwas weißt. Du baust seit
  Monaten eine Trainings-App — du weißt mehr über progressive Steigerung
  als die meisten dort.
- Wenn jemand nach einer Tracker-App fragt — und das passiert regelmäßig —
  antwortest du **ehrlich mit allen Optionen** und nennst IRON als eine
  davon, mit dem Bild aus Abschnitt 3 und dem Zusatz "ist von mir, noch
  früh, kostet gerade nichts".

Diese Ehrlichkeit ist nicht Anstand, sondern Taktik: In solchen Gruppen
riecht man Werbung sofort. "Ist von mir und noch früh" macht dich vom
Verkäufer zum Bastler — und Bastlern hilft man gern.

## 7. Was gebaut werden muss

Marketing baut nichts. Diese Anforderungen gehen an die zuständigen
Baustellen und wandern in `docs/stand.md`.

**A1 — Die Link-Vorschau reparieren.** *(dringend, alles hängt daran)*
`index.html` enthält im Kopf nur `<title>IRON</title>` — keine Beschreibung,
kein Vorschaubild. Jeder geteilte Link erzeugt daher ein leeres graues
Kästchen. Das trifft das Empfehlungsprogramm (`shareInvite()`) und die
App-Adresse auf der Sieger-Bildkarte, also beide bereits gebauten
Wachstums-Werkzeuge. **Der Integrator repariert das.**

Die Texte dafür, fertig zum Einsetzen:

| Feld | Inhalt |
|---|---|
| Beschreibung / `og:description` | Andere Trainings-Apps geben dir ein leeres Feld. IRON hat die Zahl schon eingetragen — es merkt sich, was du letztes Mal gehoben hast. |
| `og:title` | IRON — Training, das mitdenkt |
| `og:image` | 1200 × 630 Pixel, quer |
| Dazu | `og:url`, `og:type` (website), `og:locale` (de_DE), `twitter:card` als große Bildkarte |

Fürs Bild braucht es nichts Neues: Die erste Willkommens-Karte — das Telefon
mit "HEUTE AUF DEM PLAN" vor dem Studio-Hintergrund — ist bereits genau das
richtige Bild. Sie muss nur ins Querformat gebracht werden. Wichtig: Das
Vorschaubild wird von den Diensten zwischengespeichert; nach einer Änderung
kann es Tage dauern, bis alle es neu holen. Also einmal richtig machen.

**A2 — "Auf den Startbildschirm legen".** *(dringend)*
Wer IRON auf einem iPhone im Browser öffnet, bekommt einen kurzen Hinweis,
wie man die App auf den Startbildschirm legt, mit Bild vom Teilen-Knopf.
Ohne das bleibt IRON eine Website und wird vergessen. Einmal zeigen, dann
nie wieder.

**A3 — Was kostet es, und brauche ich ein Konto?** *(Wachstum)*
Nirgends im Einstieg wird beantwortet, was IRON kostet und ob ein Konto
nötig ist. Das sind die zwei Fragen, die jeder Fremde stellt, bevor er
irgendetwas antippt — und wer keine Antwort findet, vermutet das Schlechtere.

Der eigentliche Punkt: **Beide Antworten sind längst entschieden und beide
sprechen für IRON.** Der Commit `0ae0976` vom 2026-09-08 hält fest, dass
IRON local-first ist und kein Konto erzwingt; ein Gratis-Monat ist im
Einstieg ebenfalls schon vorgesehen. Da wird ein starkes Verkaufsargument
gebaut und niemandem gesagt — und zwar genau das Argument, das dich von MCI
trennt, wo ohne Konto und Coaching-Abo gar nichts läuft.

Ein Satz an der richtigen Stelle genügt: *ohne Konto starten, IRON+ kostet
4,99 € im Monat oder 39,99 € im Jahr, der erste Monat ist frei.* Keine
Preistabelle, kein eigener Bildschirm. Die genaue Formulierung liefert
Marketing, sobald die Baustelle Wachstum sagt, wohin sie passt — der
Einstieg wird gerade ohnehin umgebaut, das gehört in denselben Durchgang.

**A4 — Empfehlen im Moment des Erfolgs, nicht in den Einstellungen.**
Das Empfehlungsprogramm läuft (`src/lib/referral.ts`, 14 Tage für beide,
30 weitere wenn der Geworbene kauft). Aber niemand geht in die
Einstellungen, um jemanden einzuladen. Angeboten werden muss es dort, wo
gerade Stolz entsteht: nach einem neuen Rekord, nach einer vollen Woche.
Das ist der billigste Wachstums-Hebel, den es gibt — er ist schon bezahlt
und wird gerade nicht benutzt.

**A5 — Die öffentliche Rangliste erst ab genug Teilnehmern zeigen.**
Eine öffentliche Rangliste mit sieben Namen ist kein Anreiz, sie ist ein
Beweis, dass niemand die App benutzt. Bitte prüfen, ob es eine
Mindestteilnehmerzahl gibt, und falls nicht: eine einbauen. Darunter lieber
den eigenen Fortschritt zeigen als eine leere Liste.

**A6 — Vor jedem Werbe-Screenshot: der Vorschlag muss echt sein.**
Keine Anforderung an Code, sondern eine Absprache. Kein Bild mit erfundenen
Zahlen, nie. Siehe Abschnitt 3.

## 8. Was wir bewusst nicht tun

Diese Liste ist genauso wichtig wie der Plan. Ein Einzelkämpfer verliert
nicht an der falschen Idee, sondern an fünf gleichzeitigen richtigen.

- **Kein eigener Instagram- oder TikTok-Kanal.** Ohne Gesicht und mit 2
  Stunden pro Woche entsteht ein Kanal mit elf Beiträgen und vierzig
  Followern, der drei Monate still steht. Das sieht schlechter aus als gar
  kein Kanal. Wenn ein Konto reserviert werden soll, damit der Name nicht
  weg ist: anlegen, ein Bild, Link in die Biografie, fertig — und dann
  liegen lassen, ohne schlechtes Gewissen.
- **Keine bezahlte Werbung.** Unter 100 € im Monat kauft man keine Nutzer,
  man kauft eine Lernerfahrung, die man sich nicht leisten kann.
- **Keine Influencer.** Ausführlich begründet in
  `docs/marketing-influencer.md`. Kurzfassung: Es ist rechnerisch nicht
  bezahlbar, technisch nicht abrechenbar, und es bringt Masse, wo du
  Feedback brauchst.
- **Noch kein App Store.** Entscheidung des Nutzers vom 2026-09-08: erst
  die Web-Version. Die vorbereiteten Store-Texte liegen fertig in
  `docs/marketing-appstore.md` und warten dort.
- **Keine eigene Werbe-Startseite.** Entscheidung des Nutzers vom
  2026-09-08: Die App ist die Demo. Der Willkommens-Screen zeigt echte
  Aufnahmen statt Werbeversprechen und leistet damit mehr als eine
  Landingpage. Was fehlt, ist nur die Vorschau davor (A1).
- **Kein Newsletter, keine Presse, kein Blog.** Alles drei kostet
  Dauerpflege und zahlt frühestens in einem Jahr zurück.
- **IRON TIMES bleibt vorerst nach innen gerichtet.** Die App-eigene Zeitung
  ist gut für die Bindung derer, die schon da sind. Neue Nutzer bringt sie
  nicht, solange sie nur in der App steht. Nicht anfassen, nicht bewerben,
  einfach laufen lassen.

## 9. Woran wir merken, ob es funktioniert

Nicht an Anmeldungen. Anmeldungen sind die Zahl, mit der man sich selbst
belügt.

Die einzige Zahl, die in diesen zwölf Wochen zählt:

> **Wie viele Menschen trainieren drei Wochen nach ihrer Anmeldung noch
> mit IRON?**

Liegt die unter einem Fünftel, ist jedes weitere Marketing rausgeworfenes
Geld und rausgeworfene Zeit — dann ist die Antwort nicht "mehr Werbung",
sondern "warum hören sie auf".

Ein ehrliches Ziel für den 8. Dezember 2026:

| | Ziel |
|---|---|
| Haben IRON ausprobiert | 30 Menschen |
| Trainieren nach 4 Wochen noch damit | 10 Menschen |
| Ausführliche Rückmeldung gegeben | 5 Menschen |
| Zahlende Abos | **0 sind in Ordnung** |

Die letzte Zeile ist ernst gemeint. In dieser Phase Geld verlangen zu wollen
lenkt nur vom Ziel ab. Die Abos kommen, wenn feststeht, dass Leute bleiben.

## 10. Was noch offen ist

Fragen, die diese Strategie schärfen würden, für die mir aber die Antwort
fehlt:

- **Was hat dich an MCI gestört, als du es dir angesehen hast?** Deine
  eigene Verärgerung ist meist der beste Werbetext.
- **Benutzt einer deiner fünf Freunde IRON heute schon regelmäßig?** Falls
  ja: Warum? Falls nein: Das ist wichtiger als jede Strategie hier.
- **Gibt es eine Datenschutzerklärung und ein Impressum?** Sobald du in
  Foren wirbst und Anmeldungen einsammelst, brauchst du beides. Das ist
  keine Marketing-Frage, aber es fällt in dem Moment auf die Füße, in dem
  Marketing anfängt zu wirken.
