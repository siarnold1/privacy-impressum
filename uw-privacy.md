**English** · [Deutsch](#datenschutzerklärung--urban-whispers)

# Privacy Policy — Urban Whispers

**Effective date:** November 2, 2026 · applies to Urban Whispers version 1.1 and later

Urban Whispers ("the App", "we") is an audio city guide with a city game: you listen to stories, collect stamps, solve riddles, plan trips and save places. **Every feature works without an account; version 1.1 has no sign-in.** This policy explains which data the App processes, why, how long it is kept, and what your rights are.

**Controller:** Simon Arnold, Landsberger Straße 119, 80339 München, Germany · simon.arnold@mailbox.org. We have not appointed a data protection officer, as we are not required to.

---

## 1. The Short Version

- **Sign-in comes later.** Version 1.1 has no sign-in yet. Your game progress, saved places and trips stay on your iPhone and are not sent to us. We plan to offer an optional sign-in with Apple or Google in a later version; Sections 3.1 and 3.2 describe what will apply then.
- **Your location stays on your device.** The Nearby tab uses your location only while it is open, and the distances are calculated on your iPhone. Your coordinates are never sent to us, never stored and never logged.
- **Your photos, notes and trip documents stay on your device.** They are never uploaded, not even when you are signed in.
- **Usage statistics only with your consent.** The App asks you once ("Help improve Urban Whispers"). Only if you allow it does it send a few pseudonymous usage events. You can withdraw your consent at any time in **Settings › Privacy** (details in 3.3).
- **Crash reports can be turned off.** Crash reports help us fix errors. They are on by default and you can turn them off in **Settings › Privacy** (details in 3.4).
- **No advertising, no cross-app tracking.** We do not use advertising or tracking SDKs, and we do not access the advertising identifier (IDFA).
- **Delete any time.** Your progress, trips, photos and notes live on your iPhone; deleting them in the App or uninstalling the App removes them. Once accounts are available, Settings › Account › Delete account will delete your account and all data stored for it on our servers.

---

## 2. Data We Do Not Collect

We do not collect, request or store:

- Your GPS position or other location data on our servers (see Section 4)
- Your photos or their metadata (see Section 5)
- Your notes and trip documents (see 3.7)
- Phone numbers, postal addresses or payment data
- Contacts, microphone recordings or other files on your device
- Your Apple or Google password. Sign-in happens in Apple's or Google's own dialog.
- Advertising identifiers (IDFA) or any other lasting device identifier. The App does not show the App Tracking Transparency prompt because it does not track you.

---

## 3. Data We Do Process

### 3.1 Account (planned for a later version)

**Not available in version 1.1.** The App currently offers no sign-in, so we do not receive or store any of the data listed in this section. It describes what will apply once we offer an optional sign-in.

You can sign in with **Sign in with Apple** or **Google** (Settings › Account, the "Back up your progress" card in the Passport, or the one-time "Keep your stamps safe" hint). Signing in is never required. If you sign in, we receive and store:

- **A user ID** that our backend creates for your account.
- **Your email address.** With Sign in with Apple you can choose "Hide My Email"; we then only receive a private Apple relay address (…@privaterelay.appleid.com), and the App shows "Hidden email".
- **The sign-in provider** (Apple or Google) and the account identifier the provider gives us for the App.
- **Your name, only if the provider shares it.** Apple shares your name only on your first sign-in and only if you allow it. Google includes your name and a link to your profile picture in its sign-in data. We do not display or use your name or picture.
- **Technical sign-in data:** the time of sign-up and of your last sign-ins, and the IP address of sign-in requests, which our sign-in service (Supabase Auth) records for security purposes.
- **Sign in with Apple only: an Apple refresh token.** We keep it on our server for one purpose only: to revoke the App's access to your Apple ID when you delete your account.

Your login session (access and refresh tokens) is stored in the iOS Keychain on your iPhone.

We do not use your email address for newsletters or marketing.

### 3.2 Sync (only when signed in, planned for a later version)

**Not available in version 1.1** (see 3.1). Nothing is synced; your data stays on your iPhone.

When you are signed in, the App backs up the following data to your account and keeps it in sync across your devices:

- **Game progress:** events such as collected stamps, completed challenges, riddle answers, used hints, solved riddles and unlocked badges. Each event has a time, the attraction, riddle or city it belongs to, and the XP it earned. Your level, streaks and badges are calculated from these events.
- **Saved places (Bucket List):** which places and episodes you saved, with a short snapshot (title, city) and the time you saved or removed them.
- **Trips:** the city, start date, number of days, your day plan, whether the morning-plan reminder is on, and when the trip was created or changed. This includes the names of **your own places** that you add to a trip (free text, up to 80 characters). Please keep in mind that free text can contain personal information if you type it in.

When you remove a saved place or a trip, it is marked as deleted so the removal also reaches your other devices. These markers are removed when you delete your account.

The App syncs when you sign in, when you open the App, when your connection comes back, and a few seconds after you change something. Each account can only read and write its own data; the database enforces this.

**Not synced:** your photos, notes, trip documents, downloaded episodes, cached content and your location.

**Storage location:** Our database is hosted by Supabase Inc. on servers in **Frankfurt, Germany (EU)**.

### 3.3 Usage Statistics (only with your consent)

Usage statistics help us understand which features are used and which riddles are too hard. They are **only collected if you agree**:

- **Asking you once.** After you finish your first episode or pass your first challenge, the App shows the sheet **"Help improve Urban Whispers"** with two equal choices. Your answer is saved, and the sheet does not appear again.
- **Changing your mind.** You can turn usage statistics on or off at any time with the switch **"Share anonymous usage statistics"** in **Settings › Privacy**. Withdrawing your consent is as easy as giving it.
- **Without your consent, nothing is stored or sent.** If you choose "No thanks" or later turn the switch off, the App stops collecting immediately and deletes the events on your iPhone that have not been sent yet. Withdrawing consent does not affect events that were sent before.

If you agree, the App sends these usage events:

- a stamp was collected
- a challenge was failed
- a riddle was solved
- a trip was created
- Nearby was opened (at most once per day)
- a sign-in happened (with the provider, Apple or Google)

Each event contains only the event type, content IDs and simple counters (for example which attraction, whether an answer was correct, which attempt it was) and a **random session ID**. The App creates a new session ID every time it starts, so sessions cannot be connected to each other or to your device. We therefore describe this data as **pseudonymous**: it is not linked to your name, your email address, your account or any lasting identifier.

- Events **never** contain your location, email address or name. Our server also removes any location, email or name fields before it stores an event.
- Events are **never connected to your account**, not even when you are signed in.
- If you are offline, up to 50 events wait on your iPhone and are sent later.
- With your consent, the App also sends anonymous app-session stability data to Sentry (see 3.4).

We look at this data only in aggregate. Usage events are stored for **24 months** and then deleted automatically.

### 3.4 Crash Reports

If the App crashes or runs into an error, a technical report is sent to Sentry (Functional Software, Inc.) so we can find and fix the problem. Crash reports contain:

- Device model and operating system version
- App version
- Technical information about the error (stack trace)

Crash reports are configured to **exclude personal information**: they contain neither names nor email addresses, account IDs or user profiles. Before a report leaves your iPhone, the App also removes coordinates and web-address parameters. To deliver a report, Sentry's servers technically receive your IP address; Sentry is configured not to store it. Crash data is processed on Sentry's **EU infrastructure (Germany)** and deleted after **90 days**.

- **Switch "Send crash reports"** in **Settings › Privacy**: on by default. Turning it off takes effect immediately for the rest of the session. Turning it back on takes effect the next time you start the App.
- **Limitation:** if the App crashed before you turned the switch off, the report for that crash may still be stored on your iPhone. It is only sent if you turn the switch on again.
- **App-session stability data** (whether App sessions end normally or with a crash, also called release health) is only sent if you have agreed to usage statistics (3.3). If you withdraw that consent, sending it stops immediately.

### 3.5 Address Search (trip planner)

In the trip planner you can search for the place where you are staying ("Where are you staying?"). The text you type, together with the name of the city, is sent to **Apple's geocoding service** (the address search built into iOS) to find matching addresses. This does not require location permission. The App does not send this text to us and does not store the text or the result; it is only kept in memory while you search. Apple processes the request under its own privacy policy.

### 3.6 Loading Content

When you browse, the App loads cities, episodes, audio, images, quizzes and riddles from our backend (Supabase). These requests do not contain personal data. Like any server on the internet, the server technically receives your IP address to answer the request; we do not use it to identify you.

### 3.7 Data Stored Only on Your Device

The following stays on your iPhone. It is never sent to us and is deleted when you uninstall the App:

- Downloaded episodes, listening progress and cached content
- Your photos (see Section 5)
- **Your notes** on attractions and trip days, and **your trip documents** (for example tickets or bookings you add to a trip). They are never synced and stay on the device when you sign out.
- As a guest: your game progress, Bucket List and trips. With an account, a copy is also synced (3.2).
- Your privacy choices (usage statistics and crash reports).
- **Morning-plan reminders.** These are local notifications scheduled on your iPhone. The App does not use push notifications and sends no push token to us or to anyone else.

---

## 4. Location (Nearby)

- The App asks for location access ("While Using the App") only when you tap the button in the Nearby tab. It never uses your location in the background.
- Your location is only used while the Nearby tab is open and the App is in the foreground. When you leave the tab or the App, it stops.
- The App downloads one list of all published attractions. The list is the same for every user, and the request does not include your position. The distances are calculated **on your iPhone**.
- Your coordinates are **never sent** to our servers, to usage statistics or to crash reports. They are **never stored**, not on your iPhone and not on a server, and they are **never logged**. Crash reports are additionally filtered for coordinates.
- You can deny or withdraw location access at any time in the iOS Settings. Every other feature keeps working.

---

## 5. Photos

- You can add your own photos to a city or trip. The App uses the iOS photo picker, so it only receives the photos you pick and has no access to the rest of your library.
- The App saves an **unchanged copy** of each picked photo in its own folder on your iPhone. The copy keeps the metadata your photo already has, such as the capture date and, if your camera recorded it, the location where it was taken.
- The App reads **only the capture date**, to sort your photos. It never reads, stores or sends the location from your photos.
- Photos are **never uploaded**, not even when you are signed in, and they are not synced. Signing out or deleting your account does not delete them. They are deleted when you delete them in the App or uninstall the App.
- If you use iCloud Backup or a computer backup for your iPhone, the App's photo folder is part of that personal backup, which is handled by Apple. We have no access to it.
- When you share a trip recap, the App creates a new image without photo metadata. It is shared only through the iOS share sheet, to the place you choose.

---

## 6. AI-Generated Content

The episodes in Urban Whispers are made with the help of artificial intelligence: the voices of Felix and Sophie are AI-generated (ElevenLabs), our stories are researched and written with the help of AI, and the images of cities and attractions are AI-generated. **Every episode is reviewed by us before it is published.**

**Your data is not processed by AI.** The App does not send your inputs, your progress or any other personal data to an AI service; AI is only used by us when we produce the content.

More about how the content is made, and how to report an error, is on the page **"About the content"** in the App (Settings › About the content, and the About tab of every episode).

---

## 7. Why We Process This Data (Legal Basis)

| Processing | Legal basis |
|---|---|
| **Account, sync and account deletion** (3.1, 3.2, Section 9), including storing the Apple token so we can revoke it on deletion | Performance of the service you asked for: **Art. 6(1)(b) GDPR** |
| **Usage statistics** (3.3) and **app-session stability data** sent to Sentry (3.4) | Your **consent**: **Art. 6(1)(a) GDPR**; storing and reading this information on your device: **§ 25(1) TDDDG**. You can withdraw your consent at any time (Art. 7(3) GDPR) in Settings › Privacy. |
| **Crash reports** (3.4) | Our **legitimate interest** in keeping the App stable and finding and fixing errors: **Art. 6(1)(f) GDPR**; the device access needed for this: **§ 25(2) No. 2 TDDDG**. You can object (Section 10) or simply turn the switch off. |
| **Loading content and operating the backend** (3.6), including the technical processing of IP addresses | Our **legitimate interest** in delivering the content you request and keeping our servers secure: **Art. 6(1)(f) GDPR**; **§ 25(2) No. 2 TDDDG** |
| **Storage on your device** (3.7) | Only what the App needs to provide the features you use: **§ 25(2) No. 2 TDDDG** |
| **Location, photos and address search** (Sections 4, 5 and 3.5) | Processed only on your iPhone or sent directly to Apple, and only when you use the feature (with your permission where iOS asks for it). We do not receive this data. |

**You are not required to provide any personal data.** Every feature works without an account; if you do not sign in, we cannot back up your progress. We do not use automated decision-making, including profiling, within the meaning of Art. 22 GDPR.

---

## 8. Recipients, Service Providers and Third Countries

We do **not sell** data, do **not share** it with advertisers and do **not track** you across other apps or websites. We use these providers:

| Provider | Purpose | Location / role |
|---|---|---|
| Supabase Inc. | Database, sign-in, sync, usage statistics, content delivery | Servers in Frankfurt, Germany (EU); processor under a data processing agreement |
| Sentry (Functional Software, Inc.) | Crash reports, app-session stability data | EU infrastructure (Germany); processor under a data processing agreement |
| Apple Inc. / Apple Distribution International Ltd. | Address search (3.5); Sign in with Apple once available (3.1) | Apple processes this data as an independent controller under its own privacy policy |
| Google (Google Ireland Ltd. / Google LLC) | Sign in with Google once available (3.1) | Google processes your sign-in as an independent controller under its own privacy policy |

**Third countries:** Supabase Inc. and Functional Software, Inc. are companies based in the USA. We use their EU hosting. Where data could still be accessed from outside the EU, the transfer is covered by the **EU-U.S. Data Privacy Framework** (where the provider is certified) and/or the **EU Standard Contractual Clauses**, which are part of the data processing agreements.

---

## 9. Data Retention, Sign-out and Account Deletion

Version 1.1 has no sign-in, so the rows on accounts and synced data, sign-out and account deletion apply only once accounts are available (see 3.1).

| Data | How long |
|---|---|
| Account and synced data (3.1, 3.2) | As long as your account exists; deleted immediately when you delete your account |
| Server backups | Deleted data can remain in our provider's encrypted backups for a short time until those backups are overwritten |
| Usage events (3.3) | **24 months**, then deleted automatically. Events not yet sent are deleted from your iPhone when you withdraw consent. |
| Crash reports and app-session stability data (3.4) | **90 days**, then deleted automatically by Sentry |
| Data on your device (3.7, Sections 4, 5) | Under your control; deleted when you delete it in the App or uninstall the App |

- **Sign-out:** the App first syncs your latest progress. If that is not possible (for example offline), it asks whether you want to sign out anyway. It then ends your session and resets game progress, Bucket List, trips and riddle progress **on this iPhone** to an empty guest state. Downloads, photos, notes and trip documents stay. Your data remains in your account, and signing in again restores it.
- **Account deletion:** in the App under **Settings › Account › Delete account** (you confirm by typing DELETE). We then delete immediately:
  - your account (user ID, email address, name, sign-in identities)
  - all synced data (game events, Bucket List, trips)
  - riddle progress and riddle reward claims
  - any usage events that were ever stored with your user ID (earlier versions; today usage events are never linked to an account)
  - your Apple refresh token. Before deleting it, we ask Apple to revoke it, so Urban Whispers no longer appears under "Sign in with Apple" in your Apple ID settings.

  Deletion cannot be undone. On your iPhone, the App switches back to a guest state; photos, notes, trip documents and downloads stay on the device. If you signed in with Google, you can also remove the App's access in your Google account (Security › Third-party connections).

---

## 10. Your Rights

Under the GDPR you have the following rights regarding your personal data:

- **Access** (Art. 15 GDPR): you can ask which data we hold about you and receive a copy.
- **Rectification** (Art. 16 GDPR): you can ask us to correct inaccurate data.
- **Erasure** (Art. 17 GDPR): you can ask us to delete your data. With an account, you can do this yourself in the App (Section 9).
- **Restriction of processing** (Art. 18 GDPR): you can ask us to limit how we use your data.
- **Data portability** (Art. 20 GDPR): you can ask for the data you gave us in a structured, commonly used, machine-readable format.
- **Withdrawing consent** (Art. 7(3) GDPR): you can withdraw your consent to usage statistics at any time in **Settings › Privacy**. This does not affect the lawfulness of processing before the withdrawal.
- **Complaint to a supervisory authority** (Art. 77 GDPR): you can complain to any data protection authority. The authority responsible for us is the **Bavarian Data Protection Authority (BayLDA)**, Bayerisches Landesamt für Datenschutzaufsicht, Promenade 18, 91522 Ansbach, Germany, https://www.lda.bayern.de.

**How to make a request:** email simon.arnold@mailbox.org. With an account, write from the address of your account, or tell us which address the App shows under Settings › Account. Without an account, the data we hold is not linked to you, so we usually cannot find "your" data; usage events in particular only carry a random session ID.

> **Right to object (Art. 21 GDPR)**
>
> Where we process your data on the basis of our legitimate interests (Art. 6(1)(f) GDPR, see Section 7, in particular crash reports), **you have the right to object at any time**, on grounds relating to your particular situation. We will then stop this processing unless we can demonstrate compelling legitimate grounds that override your interests, rights and freedoms, or the processing serves the establishment, exercise or defence of legal claims.
>
> The easiest way to object to crash reports is to turn off **"Send crash reports"** in **Settings › Privacy**. You can also send your objection informally by email to simon.arnold@mailbox.org.

---

## 11. Children

Urban Whispers is suitable for general audiences, and every feature can be used without an account. We do not knowingly collect personal data from children. Sign-in is provided by Apple and Google under their own age rules.

---

## 12. Changes to This Policy

If we change how the App handles data, we will update this policy before the change goes live and show the new effective date at the top of this page.

---

## 13. Contact

If you have questions about this policy or your data:

**Simon Arnold**
Landsberger Straße 119, 80339 München, Germany
**Email:** simon.arnold@mailbox.org

We have not appointed a data protection officer.

Imprint / legal notice: [Legal notice](https://github.com/siarnold1/privacy-impressum/blob/main/uw-impressum.md)

---

[English](#privacy-policy--urban-whispers) · **Deutsch**

# Datenschutzerklärung – Urban Whispers

**Gültig ab:** 2. November 2026 · gilt für Urban Whispers ab Version 1.1

Urban Whispers („die App“, „wir“) ist ein Audio-Stadtführer mit Stadtspiel: Du hörst Geschichten, sammelst Stempel, löst Rätsel, planst Reisen und merkst Dir Orte. **Jede Funktion funktioniert ohne Konto; Version 1.1 bietet keine Anmeldung.** Diese Erklärung beschreibt, welche Daten die App verarbeitet, warum, wie lange sie gespeichert werden und welche Rechte Du hast. Die englische und die deutsche Fassung sind inhaltlich gleich; die Namen von Schaltern und Seiten stehen auf Englisch, so wie sie in der App erscheinen.

**Verantwortlicher:** Simon Arnold, Landsberger Straße 119, 80339 München, Deutschland · simon.arnold@mailbox.org. Ein Datenschutzbeauftragter ist nicht bestellt, da keine Pflicht dazu besteht.

---

## 1. Kurzfassung

- **Anmeldung kommt später.** Version 1.1 bietet noch keine Anmeldung. Dein Spielfortschritt, Deine gemerkten Orte und Reisen bleiben auf Deinem iPhone und werden nicht an uns gesendet. Eine freiwillige Anmeldung mit Apple oder Google planen wir für eine spätere Version; die Abschnitte 3.1 und 3.2 beschreiben, was dann gilt.
- **Dein Standort bleibt auf Deinem Gerät.** Der Tab „Nearby“ nutzt Deinen Standort nur, solange er geöffnet ist; die Entfernungen werden auf Deinem iPhone berechnet. Deine Koordinaten werden nie an uns gesendet, nie gespeichert und nie protokolliert.
- **Deine Fotos, Notizen und Reise-Dokumente bleiben auf Deinem Gerät.** Sie werden nie hochgeladen, auch nicht, wenn Du angemeldet bist.
- **Nutzungsstatistik nur mit Deiner Einwilligung.** Die App fragt Dich einmal („Help improve Urban Whispers“). Nur wenn Du zustimmst, sendet sie einige pseudonyme Nutzungsereignisse. Den Widerruf kannst Du jederzeit unter **Settings › Privacy** erklären (Details in 3.3).
- **Absturzberichte lassen sich abschalten.** Absturzberichte helfen uns, Fehler zu beheben. Sie sind standardmäßig an und lassen sich unter **Settings › Privacy** ausschalten (Details in 3.4).
- **Keine Werbung, kein app-übergreifendes Tracking.** Wir nutzen keine Werbe- oder Tracking-SDKs und greifen nicht auf die Werbe-ID (IDFA) zu.
- **Jederzeit löschen.** Fortschritt, Reisen, Fotos und Notizen liegen auf Deinem iPhone; Du löschst sie in der App oder indem Du die App entfernst. Sobald es Konten gibt, löscht Settings › Account › Delete account Dein Konto und alle dazu auf unseren Servern gespeicherten Daten.

---

## 2. Daten, die wir nicht erheben

Wir erheben, erfragen oder speichern nicht:

- Deine GPS-Position oder andere Standortdaten auf unseren Servern (siehe Abschnitt 4)
- Deine Fotos oder deren Metadaten (siehe Abschnitt 5)
- Deine Notizen und Reise-Dokumente (siehe 3.7)
- Telefonnummern, Postanschriften oder Zahlungsdaten
- Kontakte, Mikrofonaufnahmen oder andere Dateien auf Deinem Gerät
- Dein Apple- oder Google-Passwort. Die Anmeldung läuft im eigenen Dialog von Apple bzw. Google.
- Werbe-IDs (IDFA) oder andere dauerhafte Gerätekennungen. Die App zeigt keine App-Tracking-Transparency-Abfrage, weil sie Dich nicht trackt.

---

## 3. Daten, die wir verarbeiten

### 3.1 Konto (für eine spätere Version geplant)

**In Version 1.1 nicht verfügbar.** Die App bietet derzeit keine Anmeldung; wir erhalten und speichern daher keine der in diesem Abschnitt genannten Daten. Er beschreibt, was gilt, sobald wir eine freiwillige Anmeldung anbieten.

Du kannst Dich mit **Sign in with Apple** oder **Google** anmelden (Settings › Account, die Karte „Back up your progress“ im Passport oder der einmalige Hinweis „Keep your stamps safe“). Eine Anmeldung ist nie erforderlich. Wenn Du Dich anmeldest, erhalten und speichern wir:

- **Eine Nutzer-ID**, die unser Backend für Dein Konto anlegt.
- **Deine E-Mail-Adresse.** Bei Sign in with Apple kannst Du „E-Mail-Adresse verbergen“ wählen; wir erhalten dann nur eine private Apple-Weiterleitungsadresse (…@privaterelay.appleid.com), und die App zeigt „Hidden email“.
- **Den Anmeldedienst** (Apple oder Google) und die Kennung, die der Anbieter uns für die App übermittelt.
- **Deinen Namen, nur wenn der Anbieter ihn übermittelt.** Apple übermittelt den Namen nur bei der ersten Anmeldung und nur, wenn Du es erlaubst. Google übermittelt Namen und einen Link zum Profilbild in den Anmeldedaten. Wir zeigen Namen und Bild nicht an und nutzen sie nicht.
- **Technische Anmeldedaten:** den Zeitpunkt der Registrierung und der letzten Anmeldungen sowie die IP-Adresse von Anmeldeanfragen, die unser Anmeldedienst (Supabase Auth) aus Sicherheitsgründen protokolliert.
- **Nur bei Sign in with Apple: ein Apple-Refresh-Token.** Wir speichern es auf unserem Server nur für einen Zweck: um beim Löschen Deines Kontos den Zugriff der App auf Deine Apple-ID zu widerrufen.

Deine Anmeldesitzung (Access- und Refresh-Token) wird im iOS-Schlüsselbund auf Deinem iPhone gespeichert.

Wir nutzen Deine E-Mail-Adresse nicht für Newsletter oder Werbung.

### 3.2 Synchronisierung (nur mit Anmeldung, für eine spätere Version geplant)

**In Version 1.1 nicht verfügbar** (siehe 3.1). Es wird nichts synchronisiert; Deine Daten bleiben auf Deinem iPhone.

Wenn Du angemeldet bist, sichert die App folgende Daten in Deinem Konto und hält sie auf Deinen Geräten synchron:

- **Spielfortschritt:** Ereignisse wie gesammelte Stempel, abgeschlossene Challenges, Rätselantworten, genutzte Tipps, gelöste Rätsel und freigeschaltete Abzeichen. Jedes Ereignis enthält einen Zeitpunkt, die zugehörige Attraktion, das Rätsel oder die Stadt und die dafür erhaltenen XP. Level, Serien und Abzeichen werden aus diesen Ereignissen berechnet.
- **Gemerkte Orte (Bucket List):** welche Orte und Episoden Du gemerkt hast, mit einer kurzen Momentaufnahme (Titel, Stadt) und dem Zeitpunkt des Merkens oder Entfernens.
- **Reisen:** Stadt, Startdatum, Anzahl der Tage, Dein Tagesplan, ob die Morgen-Erinnerung an ist und wann die Reise angelegt oder geändert wurde. Dazu gehören auch die Namen **eigener Orte**, die Du einer Reise hinzufügst (Freitext, bis 80 Zeichen). Bitte bedenke, dass Freitext personenbezogene Angaben enthalten kann, wenn Du sie eintippst.

Wenn Du einen gemerkten Ort oder eine Reise entfernst, wird der Eintrag als gelöscht markiert, damit das Entfernen auch Deine anderen Geräte erreicht. Diese Markierungen werden beim Löschen Deines Kontos entfernt.

Die App synchronisiert bei der Anmeldung, beim Öffnen der App, wenn die Verbindung zurückkommt, und einige Sekunden nach einer Änderung. Jedes Konto kann nur seine eigenen Daten lesen und schreiben; die Datenbank setzt das durch.

**Nicht synchronisiert:** Deine Fotos, Notizen, Reise-Dokumente, geladenen Episoden, zwischengespeicherte Inhalte und Dein Standort.

**Speicherort:** Unsere Datenbank wird von Supabase Inc. auf Servern in **Frankfurt (EU)** betrieben.

### 3.3 Nutzungsstatistik (nur mit Deiner Einwilligung)

Die Nutzungsstatistik hilft uns zu verstehen, welche Funktionen genutzt werden und welche Rätsel zu schwer sind. Sie wird **nur erhoben, wenn Du einwilligst**:

- **Einmalige Frage.** Nachdem Du Deine erste Episode zu Ende gehört oder Deine erste Challenge bestanden hast, zeigt die App das Fenster **„Help improve Urban Whispers“** mit zwei gleichwertigen Antworten. Deine Antwort wird gespeichert, das Fenster erscheint danach nicht mehr.
- **Meinung ändern.** Mit dem Schalter **„Share anonymous usage statistics“** unter **Settings › Privacy** kannst Du die Nutzungsstatistik jederzeit ein- oder ausschalten. Der Widerruf ist so einfach wie die Einwilligung.
- **Ohne Einwilligung wird nichts gespeichert oder gesendet.** Wählst Du „No thanks“ oder schaltest Du den Schalter später aus, hört die App sofort auf zu erfassen und löscht die noch nicht gesendeten Ereignisse auf Deinem iPhone. Der Widerruf berührt Ereignisse, die vorher gesendet wurden, nicht.

Mit Deiner Einwilligung sendet die App diese Nutzungsereignisse:

- ein Stempel wurde gesammelt
- eine Challenge wurde nicht bestanden
- ein Rätsel wurde gelöst
- eine Reise wurde angelegt
- „Nearby“ wurde geöffnet (höchstens einmal pro Tag)
- eine Anmeldung fand statt (mit dem Anbieter, Apple oder Google)

Jedes Ereignis enthält nur den Ereignistyp, Inhalts-IDs und einfache Zähler (zum Beispiel welche Attraktion, ob eine Antwort richtig war, der wievielte Versuch es war) und eine **zufällige Sitzungs-ID**. Die App erzeugt bei jedem Start eine neue Sitzungs-ID, sodass Sitzungen weder miteinander noch mit Deinem Gerät verknüpft werden können. Wir bezeichnen diese Daten deshalb als **pseudonym**: Sie sind nicht mit Deinem Namen, Deiner E-Mail-Adresse, Deinem Konto oder einer dauerhaften Kennung verknüpft.

- Ereignisse enthalten **nie** Deinen Standort, Deine E-Mail-Adresse oder Deinen Namen. Unser Server entfernt solche Felder zusätzlich, bevor er ein Ereignis speichert.
- Ereignisse werden **nie mit Deinem Konto verknüpft**, auch nicht, wenn Du angemeldet bist.
- Ohne Internetverbindung warten bis zu 50 Ereignisse auf Deinem iPhone und werden später gesendet.
- Mit Deiner Einwilligung sendet die App außerdem anonyme Stabilitätsdaten zu App-Sitzungen an Sentry (siehe 3.4).

Wir werten diese Daten nur zusammengefasst aus. Nutzungsereignisse werden **24 Monate** gespeichert und danach automatisch gelöscht.

### 3.4 Absturzberichte

Stürzt die App ab oder tritt ein Fehler auf, wird ein technischer Bericht an Sentry (Functional Software, Inc.) gesendet, damit wir das Problem finden und beheben können. Absturzberichte enthalten:

- Gerätemodell und Version des Betriebssystems
- App-Version
- technische Angaben zum Fehler (Stacktrace)

Absturzberichte sind so eingestellt, dass sie **keine personenbezogenen Angaben** enthalten: weder Namen noch E-Mail-Adressen, Konto-IDs oder Nutzerprofile. Bevor ein Bericht Dein iPhone verlässt, entfernt die App außerdem Koordinaten und Parameter aus Webadressen. Um einen Bericht entgegenzunehmen, erhalten die Server von Sentry technisch Deine IP-Adresse; Sentry ist so eingestellt, dass sie nicht gespeichert wird. Die Daten werden auf der **EU-Infrastruktur von Sentry (Deutschland)** verarbeitet und nach **90 Tagen** gelöscht.

- **Schalter „Send crash reports“** unter **Settings › Privacy**: standardmäßig an. Das Ausschalten wirkt sofort für den Rest der Sitzung. Das Wiedereinschalten wirkt ab dem nächsten Start der App.
- **Einschränkung:** Ist die App abgestürzt, bevor Du den Schalter ausgeschaltet hast, kann der Bericht zu diesem Absturz noch auf Deinem iPhone liegen. Er wird erst gesendet, wenn Du den Schalter wieder einschaltest.
- **Stabilitätsdaten zu App-Sitzungen** (ob Sitzungen normal oder mit einem Absturz enden, sogenannte Release Health) werden nur gesendet, wenn Du in die Nutzungsstatistik eingewilligt hast (3.3). Widerrufst Du diese Einwilligung, endet auch dieses Senden sofort.

### 3.5 Adresssuche (Reiseplaner)

Im Reiseplaner kannst Du nach Deiner Unterkunft suchen („Where are you staying?“). Der eingegebene Text wird zusammen mit dem Namen der Stadt an den **Geocoding-Dienst von Apple** (die in iOS eingebaute Adresssuche) gesendet, um passende Adressen zu finden. Dafür ist keine Standortberechtigung nötig. Die App sendet den Text nicht an uns und speichert weder den Text noch das Ergebnis; beides wird nur während der Suche im Arbeitsspeicher gehalten. Apple verarbeitet die Anfrage nach seiner eigenen Datenschutzerklärung.

### 3.6 Laden von Inhalten

Beim Stöbern lädt die App Städte, Episoden, Audio, Bilder, Quizfragen und Rätsel von unserem Backend (Supabase). Diese Anfragen enthalten keine personenbezogenen Daten. Wie jeder Server im Internet erhält der Server technisch Deine IP-Adresse, um die Anfrage zu beantworten; wir nutzen sie nicht, um Dich zu identifizieren.

### 3.7 Daten, die nur auf Deinem Gerät gespeichert werden

Folgendes bleibt auf Deinem iPhone. Es wird nie an uns gesendet und beim Löschen der App entfernt:

- geladene Episoden, Hörfortschritt und zwischengespeicherte Inhalte
- Deine Fotos (siehe Abschnitt 5)
- **Deine Notizen** zu Attraktionen und Reisetagen und **Deine Reise-Dokumente** (zum Beispiel Tickets oder Buchungen, die Du einer Reise hinzufügst). Sie werden nie synchronisiert und bleiben beim Abmelden auf dem Gerät.
- als Gast: Dein Spielfortschritt, Deine Bucket List und Reisen. Mit Konto wird zusätzlich eine Kopie synchronisiert (3.2).
- Deine Datenschutz-Einstellungen (Nutzungsstatistik und Absturzberichte)
- **Morgen-Erinnerungen.** Das sind lokale Benachrichtigungen, die auf Deinem iPhone geplant werden. Die App nutzt keine Push-Benachrichtigungen und sendet kein Push-Token, weder an uns noch an andere.

---

## 4. Standort (Nearby)

- Die App fragt nach dem Standortzugriff („Beim Verwenden der App“) erst, wenn Du im Tab „Nearby“ auf den Button tippst. Sie nutzt Deinen Standort nie im Hintergrund.
- Dein Standort wird nur genutzt, solange der Tab „Nearby“ geöffnet ist und die App im Vordergrund läuft. Verlässt Du den Tab oder die App, endet die Nutzung.
- Die App lädt eine Liste aller veröffentlichten Attraktionen. Die Liste ist für alle Nutzer gleich, und die Anfrage enthält Deine Position nicht. Die Entfernungen werden **auf Deinem iPhone** berechnet.
- Deine Koordinaten werden **nie gesendet**, weder an unsere Server noch in die Nutzungsstatistik oder in Absturzberichte. Sie werden **nie gespeichert**, weder auf Deinem iPhone noch auf einem Server, und **nie protokolliert**. Absturzberichte werden zusätzlich auf Koordinaten gefiltert.
- Du kannst den Standortzugriff jederzeit in den iOS-Einstellungen verweigern oder widerrufen. Alle anderen Funktionen bleiben nutzbar.

---

## 5. Fotos

- Du kannst einer Stadt oder Reise eigene Fotos hinzufügen. Die App nutzt die iOS-Fotoauswahl; sie erhält also nur die Fotos, die Du auswählst, und hat keinen Zugriff auf den Rest Deiner Mediathek.
- Die App speichert eine **unveränderte Kopie** jedes ausgewählten Fotos in ihrem eigenen Ordner auf Deinem iPhone. Die Kopie behält die Metadaten, die Dein Foto bereits hat, etwa das Aufnahmedatum und, falls Deine Kamera ihn aufgezeichnet hat, den Aufnahmeort.
- Die App liest **nur das Aufnahmedatum**, um Deine Fotos zu sortieren. Den Aufnahmeort liest, speichert oder sendet sie nie.
- Fotos werden **nie hochgeladen**, auch nicht mit Anmeldung, und nicht synchronisiert. Abmelden oder Kontolöschung löscht sie nicht. Sie werden gelöscht, wenn Du sie in der App löschst oder die App entfernst.
- Nutzt Du iCloud-Backup oder ein Computer-Backup Deines iPhones, ist der Fotoordner der App Teil dieses persönlichen Backups, das Apple verwaltet. Wir haben darauf keinen Zugriff.
- Wenn Du einen Reiserückblick teilst, erzeugt die App ein neues Bild ohne Foto-Metadaten. Es wird nur über das iOS-Teilen-Menü an das Ziel geteilt, das Du auswählst.

---

## 6. KI-generierte Inhalte

Die Episoden von Urban Whispers entstehen mit Hilfe künstlicher Intelligenz: Die Stimmen von Felix und Sophie sind KI-generiert (ElevenLabs), unsere Geschichten werden mit Hilfe von KI recherchiert und geschrieben, und die Bilder von Städten und Attraktionen sind KI-generiert. **Jede Episode wird vor der Veröffentlichung von uns geprüft.**

**Deine Daten werden nicht durch KI verarbeitet.** Die App sendet weder Deine Eingaben noch Deinen Fortschritt oder andere personenbezogene Daten an einen KI-Dienst; KI nutzen nur wir bei der Herstellung der Inhalte.

Mehr über die Entstehung der Inhalte und wie Du Fehler melden kannst, steht in der App auf der Seite „Über die Inhalte“ (in der App: **„About the content“**, unter Settings › About the content und im About-Tab jeder Episode).

---

## 7. Warum wir diese Daten verarbeiten (Rechtsgrundlagen)

| Verarbeitung | Rechtsgrundlage |
|---|---|
| **Konto, Synchronisierung und Kontolöschung** (3.1, 3.2, Abschnitt 9), einschließlich der Speicherung des Apple-Tokens für den Widerruf bei der Löschung | Erfüllung des von Dir gewünschten Dienstes: **Art. 6 Abs. 1 lit. b DSGVO** |
| **Nutzungsstatistik** (3.3) und **Stabilitätsdaten zu App-Sitzungen** an Sentry (3.4) | Deine **Einwilligung**: **Art. 6 Abs. 1 lit. a DSGVO**; Speichern und Auslesen dieser Informationen auf Deinem Gerät: **§ 25 Abs. 1 TDDDG**. Den Widerruf kannst Du jederzeit unter Settings › Privacy erklären (Art. 7 Abs. 3 DSGVO). |
| **Absturzberichte** (3.4) | Unser **berechtigtes Interesse**, die App stabil zu halten und Fehler zu finden und zu beheben: **Art. 6 Abs. 1 lit. f DSGVO**; der dafür nötige Zugriff auf das Endgerät: **§ 25 Abs. 2 Nr. 2 TDDDG**. Du kannst widersprechen (Abschnitt 10) oder einfach den Schalter ausschalten. |
| **Laden von Inhalten und Betrieb des Backends** (3.6), einschließlich der technischen Verarbeitung von IP-Adressen | Unser **berechtigtes Interesse**, die von Dir angefragten Inhalte auszuliefern und unsere Server sicher zu betreiben: **Art. 6 Abs. 1 lit. f DSGVO**; **§ 25 Abs. 2 Nr. 2 TDDDG** |
| **Speicherung auf Deinem Gerät** (3.7) | Nur, was die App für die von Dir genutzten Funktionen braucht: **§ 25 Abs. 2 Nr. 2 TDDDG** |
| **Standort, Fotos und Adresssuche** (Abschnitte 4, 5 und 3.5) | Verarbeitung nur auf Deinem iPhone oder direkt durch Apple, und nur, wenn Du die Funktion nutzt (mit Deiner Erlaubnis, wo iOS danach fragt). Wir erhalten diese Daten nicht. |

**Du bist nicht verpflichtet, personenbezogene Daten bereitzustellen.** Jede Funktion funktioniert ohne Konto; ohne Anmeldung können wir Deinen Fortschritt nur nicht sichern. Eine automatisierte Entscheidungsfindung einschließlich Profiling im Sinne von Art. 22 DSGVO findet nicht statt.

---

## 8. Empfänger, Dienstleister und Drittländer

Wir **verkaufen keine** Daten, geben sie **nicht an Werbetreibende** weiter und **tracken Dich nicht** über andere Apps oder Websites hinweg. Wir setzen diese Dienstleister ein:

| Anbieter | Zweck | Ort / Rolle |
|---|---|---|
| Supabase Inc. | Datenbank, Anmeldung, Synchronisierung, Nutzungsstatistik, Auslieferung der Inhalte | Server in Frankfurt (EU); Auftragsverarbeiter mit Auftragsverarbeitungsvertrag |
| Sentry (Functional Software, Inc.) | Absturzberichte, Stabilitätsdaten zu App-Sitzungen | EU-Infrastruktur (Deutschland); Auftragsverarbeiter mit Auftragsverarbeitungsvertrag |
| Apple Inc. / Apple Distribution International Ltd. | Adresssuche (3.5); Sign in with Apple, sobald verfügbar (3.1) | Apple verarbeitet diese Daten als eigener Verantwortlicher nach seiner Datenschutzerklärung |
| Google (Google Ireland Ltd. / Google LLC) | Anmeldung mit Google, sobald verfügbar (3.1) | Google verarbeitet die Anmeldung als eigener Verantwortlicher nach seiner Datenschutzerklärung |

**Drittländer:** Supabase Inc. und Functional Software, Inc. haben ihren Sitz in den USA. Wir nutzen ihr Hosting in der EU. Soweit dennoch ein Zugriff von außerhalb der EU möglich ist, ist die Übermittlung durch das **EU-US Data Privacy Framework** (soweit der Anbieter zertifiziert ist) und/oder die **EU-Standardvertragsklauseln** abgesichert, die Teil der Auftragsverarbeitungsverträge sind.

---

## 9. Speicherdauer, Abmelden und Kontolöschung

Version 1.1 bietet keine Anmeldung; die Zeilen zu Konto und synchronisierten Daten sowie Abmelden und Kontolöschung gelten erst, sobald es Konten gibt (siehe 3.1).

| Daten | Wie lange |
|---|---|
| Konto und synchronisierte Daten (3.1, 3.2) | Solange Dein Konto besteht; sofortige Löschung, wenn Du Dein Konto löschst |
| Server-Backups | Gelöschte Daten können für kurze Zeit in den verschlüsselten Backups unseres Anbieters verbleiben, bis diese überschrieben werden |
| Nutzungsereignisse (3.3) | **24 Monate**, danach automatische Löschung. Noch nicht gesendete Ereignisse werden beim Widerruf auf Deinem iPhone gelöscht. |
| Absturzberichte und Stabilitätsdaten zu App-Sitzungen (3.4) | **90 Tage**, danach automatische Löschung durch Sentry |
| Daten auf Deinem Gerät (3.7, Abschnitte 4, 5) | In Deiner Hand; gelöscht, wenn Du sie in der App löschst oder die App entfernst |

- **Abmelden:** Die App synchronisiert zuerst Deinen letzten Stand. Geht das nicht (zum Beispiel offline), fragt sie, ob Du Dich trotzdem abmelden willst. Danach beendet sie die Sitzung und setzt Spielfortschritt, Bucket List, Reisen und Rätselfortschritt **auf diesem iPhone** auf einen leeren Gaststand zurück. Downloads, Fotos, Notizen und Reise-Dokumente bleiben. Deine Daten bleiben in Deinem Konto; bei erneuter Anmeldung werden sie wiederhergestellt.
- **Kontolöschung:** in der App unter **Settings › Account › Delete account** (Du bestätigst durch Eintippen von DELETE). Wir löschen dann sofort:
  - Dein Konto (Nutzer-ID, E-Mail-Adresse, Name, Anmeldeidentitäten)
  - alle synchronisierten Daten (Spielereignisse, Bucket List, Reisen)
  - Rätselfortschritt und eingelöste Rätselbelohnungen
  - Nutzungsereignisse, die jemals mit Deiner Nutzer-ID gespeichert wurden (frühere Versionen; heute werden Nutzungsereignisse nie mit einem Konto verknüpft)
  - Dein Apple-Refresh-Token. Vor dem Löschen bitten wir Apple, es zu widerrufen, sodass Urban Whispers in den Einstellungen Deiner Apple-ID nicht mehr unter „Mit Apple anmelden“ erscheint.

  Die Löschung lässt sich nicht rückgängig machen. Auf Deinem iPhone wechselt die App in den Gaststand; Fotos, Notizen, Reise-Dokumente und Downloads bleiben auf dem Gerät. Hast Du Dich mit Google angemeldet, kannst Du den Zugriff der App zusätzlich in Deinem Google-Konto entfernen (Sicherheit › Drittanbieter-Verbindungen).

---

## 10. Deine Rechte

Nach der DSGVO hast Du bezüglich Deiner personenbezogenen Daten folgende Rechte:

- **Auskunft** (Art. 15 DSGVO): Du kannst erfragen, welche Daten wir über Dich gespeichert haben, und eine Kopie erhalten.
- **Berichtigung** (Art. 16 DSGVO): Du kannst die Korrektur unrichtiger Daten verlangen.
- **Löschung** (Art. 17 DSGVO): Du kannst die Löschung Deiner Daten verlangen. Mit Konto kannst Du das in der App selbst tun (Abschnitt 9).
- **Einschränkung der Verarbeitung** (Art. 18 DSGVO): Du kannst verlangen, dass wir die Nutzung Deiner Daten einschränken.
- **Datenübertragbarkeit** (Art. 20 DSGVO): Du kannst die Daten, die Du uns bereitgestellt hast, in einem strukturierten, gängigen und maschinenlesbaren Format verlangen.
- **Widerruf der Einwilligung** (Art. 7 Abs. 3 DSGVO): Deine Einwilligung in die Nutzungsstatistik kannst Du jederzeit unter **Settings › Privacy** widerrufen. Die Rechtmäßigkeit der Verarbeitung bis zum Widerruf bleibt unberührt.
- **Beschwerde bei einer Aufsichtsbehörde** (Art. 77 DSGVO): Du kannst Dich bei jeder Datenschutzaufsichtsbehörde beschweren. Für uns zuständig ist die Aufsichtsbehörde **Bayerisches Landesamt für Datenschutzaufsicht (BayLDA)**, Promenade 18, 91522 Ansbach, https://www.lda.bayern.de.

**So stellst Du einen Antrag:** per E-Mail an simon.arnold@mailbox.org. Mit Konto schreib bitte von der Adresse Deines Kontos oder nenne uns die Adresse, die die App unter Settings › Account anzeigt. Ohne Konto sind die Daten bei uns nicht mit Dir verknüpft; wir können „Deine“ Daten daher in der Regel nicht finden, Nutzungsereignisse tragen zum Beispiel nur eine zufällige Sitzungs-ID.

> **Widerspruchsrecht (Art. 21 DSGVO)**
>
> Soweit wir Deine Daten auf Grundlage unserer berechtigten Interessen verarbeiten (Art. 6 Abs. 1 lit. f DSGVO, siehe Abschnitt 7, insbesondere Absturzberichte), **hast Du das Recht, jederzeit Widerspruch einzulegen**, aus Gründen, die sich aus Deiner besonderen Situation ergeben. Wir beenden die Verarbeitung dann, es sei denn, wir können zwingende schutzwürdige Gründe nachweisen, die Deine Interessen, Rechte und Freiheiten überwiegen, oder die Verarbeitung dient der Geltendmachung, Ausübung oder Verteidigung von Rechtsansprüchen.
>
> Am einfachsten widersprichst Du den Absturzberichten, indem Du **„Send crash reports“** unter **Settings › Privacy** ausschaltest. Du kannst den Widerspruch auch formlos per E-Mail an simon.arnold@mailbox.org richten.

---

## 11. Kinder

Urban Whispers ist für alle Altersgruppen geeignet, und jede Funktion ist ohne Konto nutzbar. Wir erheben wissentlich keine personenbezogenen Daten von Kindern. Die Anmeldung stellen Apple und Google nach ihren eigenen Altersregeln bereit.

---

## 12. Änderungen dieser Erklärung

Ändern wir, wie die App mit Daten umgeht, aktualisieren wir diese Erklärung, bevor die Änderung wirksam wird, und zeigen oben das neue Datum an.

---

## 13. Kontakt

Bei Fragen zu dieser Erklärung oder zu Deinen Daten:

**Simon Arnold**
Landsberger Straße 119, 80339 München, Deutschland
**E-Mail:** simon.arnold@mailbox.org

Ein Datenschutzbeauftragter ist nicht bestellt.

Impressum: [Impressum](https://github.com/siarnold1/privacy-impressum/blob/main/uw-impressum.md)
