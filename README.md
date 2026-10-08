# tailsync-privacy
Datenschutzerklärungen für Android und Windows

Deutsche Version

TailSync – Datenschutzerklärung
Stand: 8. Oktober 2026. Verantwortlich: Ctxch, E-Mail: cryptotxch@protonmail.com.

Kurzfassung
TailSync verbindet deine eigenen Geräte (Android-Handy und PCs) direkt miteinander. Es gibt keinen Server des Entwicklers, kein Benutzerkonto, keine Werbung, keine Analyse- oder Tracking-Dienste. Der Entwickler erhält keinerlei Daten von dir.

Welche Daten verarbeitet werden – und wohin sie gehen
Alle unten genannten Daten werden ausschließlich zwischen deinen eigenen, von dir gekoppelten Geräten übertragen – direkt über dein lokales Netzwerk oder über dein eigenes Tailscale-Netzwerk. Die Verbindung ist per TLS verschlüsselt und beide Geräte authentifizieren sich gegenseitig (Kopplung mit Fingerabdruck-Bestätigung).

• Zwischenablage (Texte und Bilder), wenn du etwas kopierst.
• Dateien, die du aktiv sendest.
• Benachrichtigungen (App-Name, Titel, Text) – nur wenn du den Benachrichtigungszugriff erteilst; Antworten, die du am PC eingibst.
• Bildschirminhalt, Kamerabild und Ton – nur während einer von dir gestarteten Bildschirmspiegelung bzw. „Handy als Webcam“-Sitzung; Android zeigt dafür jeweils eine eigene Zustimmungsabfrage.
• Eingaben zur Fernsteuerung (Mausbewegungen, Klicks, getippter Text) vom Handy zum PC.
• Geräteinformationen: Gerätename, Plattform, Akkustand, Infos zur gerade laufenden Medienwiedergabe.

Im lokalen Netzwerk sichtbar:
Damit gekoppelte Geräte sich im selben Netzwerk finden, sendet TailSync regelmäßig eine kleine Rundsendung (Broadcast) ins lokale Netzwerk mit Gerätekennung, Gerätename und Plattform. Diese ist für andere Geräte im selben lokalen Netzwerk sichtbar, enthält aber keine Inhalte.

Netzlaufwerk (optional):
Wenn du das Netzlaufwerk (WebDAV) einschaltest, kann ein PC mit Benutzername und Passwort auf den Speicher des Handys zugreifen. Diese Verbindung ist passwortgeschützt, aber nicht zusätzlich verschlüsselt (unverschlüsseltes HTTP innerhalb deines Netzwerks bzw. über Tailscale). Standardmäßig ist sie ausgeschaltet.

Speicherung
Auf jedem Gerät speichert TailSync lokal: Einstellungen, die Liste gekoppelter Geräte, den eigenen kryptografischen Schlüssel sowie empfangene Dateien im von dir gewählten Ordner (dort landen auch per Zwischenablage empfangene Bilder). Der Verlauf der Zwischenablage und gespiegelte Benachrichtigungen werden nur im Arbeitsspeicher gehalten und beim Beenden der App gelöscht. Auf Android werden durch Deinstallieren der App alle lokal gespeicherten App-Daten entfernt (empfangene Dateien in einem selbst gewählten Ordner bleiben erhalten). Unter Windows liegen die App-Daten im Ordner %USERPROFILE%\.tailsync; er bleibt beim Deinstallieren erhalten, damit eine Neuinstallation die Kopplungen behält, und kann von Hand gelöscht werden.

Berechtigungen und wofür sie genutzt werden
• Netzwerk: Verbindung zu deinen gekoppelten Geräten.
• Benachrichtigungen: Statusanzeige der Verbindung, „Handy suchen“, Abstandssperre.
• Kamera / Mikrofon: nur für „Handy als Webcam“.
• Bildschirmaufnahme: nur für die Bildschirmspiegelung, nach Zustimmung.
• Benachrichtigungszugriff: nur zum Spiegeln von Benachrichtigungen auf deinen PC.
• Zugriff auf alle Dateien: nur für das optionale Netzlaufwerk.
• Über anderen Apps einblenden: optionaler Hintergrund-Sync der Zwischenablage und Warnanzeige der Abstandssperre.
• Geräteadministrator (nur „Bildschirm sperren“): Abstandssperre und Sperren vom PC aus. TailSync löscht keine Daten und ändert keine Bildschirmsperre.

Windows-App:
• Zwischenablage: wird überwacht, solange TailSync läuft, um Änderungen an deine gekoppelten Geräte zu senden.
• Tastatur- und Mauseingaben: TailSync erzeugt Eingaben nur, wenn du den PC vom gekoppelten Handy aus steuerst; es liest keine Tastatureingaben mit.
• Medienwiedergabe: Titel, Interpret, Cover und Fortschritt der laufenden Wiedergabe werden für die Anzeige auf dem Handy ausgelesen.
• Kameratreiber (optional): Für „Handy als Webcam“ wird nach deiner Bestätigung ein virtueller Kameratreiber („TailSync Camera“) installiert. Er gibt nur das Bild deines Handys weiter und lässt sich unter „Installierte Apps“ oder in den TailSync-Einstellungen entfernen.
• Autostart (optional): nur wenn du „Beim Anmelden starten“ einschaltest.

Dienste Dritter
TailSync enthält keine Dienste Dritter. Wenn du Tailscale verwendest, ist das eine separate App mit eigener Datenschutzerklärung; TailSync nutzt lediglich das von Tailscale bereitgestellte Netzwerk.

Kinder
TailSync richtet sich nicht an Kinder.

Kontakt und Änderungen
Fragen zum Datenschutz: cryptotxch@protonmail.com. Änderungen dieser Erklärung werden auf dieser Seite veröffentlicht.


--------------------------------------------------------------------------------
English Version

TailSync – Privacy Policy
Last updated: October 8, 2026. Contact: Ctxch, cryptotxch@protonmail.com.

Summary
TailSync connects your own devices (Android phone and PCs) directly with each other. There is no developer server, no account, no ads, no analytics or tracking. The developer receives no data from you.

What data is processed – and where it goes
All data below is transferred only between your own paired devices, directly over your local network or your own Tailscale network. Connections are TLS-encrypted and both devices authenticate each other (pairing with fingerprint confirmation).

• Clipboard (text and images) when you copy something.
• Files you actively send.
• Notifications (app name, title, text) – only if you grant notification access; replies you type on the PC.
• Screen content, camera image and audio – only during a screen-mirror or phone-as-webcam session you start; Android shows its own consent prompt for each.
• Remote-control input (mouse movement, clicks, typed text) from phone to PC.
• Device information: device name, platform, battery level, currently playing media.

Visible on the local network:
So paired devices can find each other, TailSync periodically broadcasts a small message on the local network containing a device ID, device name and platform. Other devices on the same local network can see it; it contains no content.

Network drive (optional):
If you enable the network drive (WebDAV), a PC can access the phone's storage with a user name and password. It is password-protected but not additionally encrypted (plain HTTP within your network or over Tailscale). It is off by default.

Storage
Each device stores locally: settings, the list of paired devices, its own cryptographic key, and received files in the folder you choose (images received via the clipboard are saved there too). Clipboard history and mirrored notifications are kept in memory only and cleared when the app exits. On Android, uninstalling removes all locally stored app data (received files in a folder you chose remain). On Windows, app data lives in %USERPROFILE%\.tailsync; it is kept on uninstall so a reinstall keeps your pairings, and can be deleted by hand.

Permissions
Network (connect to your devices); notifications (connection status, find my phone, proximity lock); camera/microphone (phone as webcam only); screen capture (screen mirroring only, after consent); notification access (mirroring notifications to your PC only); all files access (optional network drive only); display over other apps (optional background clipboard sync and proximity-lock warning); device admin with the "lock screen" policy only (proximity lock and locking from your PC – TailSync never wipes data or changes your screen lock).

Windows app:
Clipboard: monitored while TailSync runs, to send changes to your paired devices. Keyboard and mouse: TailSync only generates input when you control the PC from your paired phone; it does not record keystrokes. Media playback: title, artist, cover art and progress of what's playing are read for display on your phone. Camera driver (optional): for "phone as webcam", a virtual camera driver ("TailSync Camera") is installed after you confirm; it only passes on your phone's image and can be removed under Installed apps or in TailSync's settings. Autostart (optional): only if you turn on "Launch at login".

Third parties
TailSync contains no third-party services. Tailscale, if you use it, is a separate app with its own privacy policy; TailSync only uses the network it provides.

Children
TailSync is not directed at children.

Contact and changes
Privacy questions: cryptotxch@protonmail.com. Changes to this policy will be published on this page.
