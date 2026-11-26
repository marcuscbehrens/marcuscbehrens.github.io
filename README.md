# icloud email mit eigener domäne für alle familienmitglieder?
Diese Seite dokumentiert wie eine Familie, die teils Apple Geräte und teils Windows oder Android Geräte benutzt, trotzdem Apple für seine email verwenden kann. Hauptvorteil ist dass der Speicher von z.Bsp. 2 TB allen zur Verfügung steht, nicht nur für emails aus Jahrzehnten sondern auch für Bilder. Und man kann seine eigene email adressen in der familie haben wie zum beispiel thomas@mueller.de und beate@mueller.de.

## Gibt es andere Optionen?

Google Workplace oder mailhoster kommen bei einer Familie mit 6 mitgliedern niemals an die 10€ für 2 TB von Apple heran. Einige meiner Verwandten haben fast 100GB email über die Jahre angesammelt und dazu noch die gleiche Menge Bilder. Gmail erlaubt ab Januar 2027 nicht mehr, dass man über einen anderen anbieter mit seiner email adresse emails verschickt. Das macht es schwieriger bei gmail als client und als email speicher zu bleiben.

## Warum ist es schwierig?

Für Familienmitglieder, die nur Apple Geräte nutzen, ist es sehr einfach. Aber auf einem Windows Rechner und auf einem Android Tablet oder Handy wirds komplizierter. Einfach nur im browser auf die icloud email gehen ist nicht so einfach weil man nur mit Apple Geräten und mit Apple Software sich nicht immer neu anmelden muss. Auf einem Windows Rechner im browser müsste man also sein passwort fast jeden Tag eingeben und auch noch per SMS einen code empfangen und eingeben. Der einzige Weg, der wirklich funktioniert sind Apps wie Thunderbird oder auch die gmail app die mit Hilfe von IMAP (Internet Message Access Protocol) die email aus der icloud abrufen und auch versenden können. Diese nutzen dafür ein passwort was in der icloud für diesen Zweck verwendet werden kann und das bei der Nutzung der app nicht mehr erfordert sich immer wieder anzumelden.

Fazit: Apple Geräte haben kein Problem, auf allen anderen Geräten muss man eine App benutzen die man einmalig installiert und aufsetzt (so wie früher), im browser auf einem beliebigen Rechner muss man sich etwas mühsamer anmelden. Dafür ist es auch etwas sicherer.

## Wie setzt man das auf und migriert die ganze Familie?

Im folgenden verwende ich "Du" wenn ein Familienmitglied etwas machen muss.

1. Alle Familienmitglieder müssen sich bei https://icloud.com/ ein Konto anlegen. Dafür auf "Anmelden" und dann auf "Neues Konto anlegen" drücken. Dafür brauchst du deine alte email Adresse und eine Handynummer. Diese Anmeldung sorgt auch dafür, dass du ein Passwort vergibst und dass bei jeder Anmeldung das Passwort und dein Handy da sein müssen.
2. Dann musst du dich mit diesem Konto einmalig auf einem ipad oder iphone oder einem Mac anmelden und wieder abmelden. Dadurch wird dein icloud konto von einem web konto auf ein vollwertiges upgegraded das auch icloud email enthält.
3. Dann wieder bei https://icloud.com/mail anmelden und eine icloud email adresse aussuchen - zum Beispiel lina.mueller@icloud.com .
4. Wenn du das alles gemacht hast teile deine alte email (die auf icloud übertragen werden soll, demjenigen mit, der das Familienkonto für alle betreiben (und auch bezahlen) soll - zum Beispiel beate@mueller.de.
5. Beate, die natürlich auch ein Apple Konto braucht, muss spätestens jetzt einen icloud plus vertrag abschliessen. Nur dann kann eine eigene domäne genutzt oder gekauft werden. Diesen gibts schon ab 1€ im Monat. Ausserdem muss sie die domäne müller.de auf icloud nutzen kann (details tbd) aber emails an die domäne weiterhin bei den nutzern auf dem alten Weg ankommt.
6. Dann lädt Beate alle Familienmitglieder in ihre Familie ein. Dies kann sie nicht auf icloud.com machen sondern nur auf einem apple Gerät. Sie kann entweder die Einladung per SMS schicken oder die Person bitten sich kurz anzumelden. Maximal 6 Familienmitglieder insgesamt mit Beate können der Familie beitreten.
7. Dann musst du die Einladung, die dir per SMS oder whatsapp geschickt wurde annehmen.
8. Dann kannst du auf https://www.icloud.com/icloudplus gehen und dir unter mueller.de eine eigene email adress anlegen - zum beispiel lina@mueller.de
9. Wenn du ein Apple Gerät hast dann kanns du auf diesem die Mail app nutzen um deine email dort zu lesen. Du kannst auch alle emails durchsuchen und emails als lina@mueller.de verschicken
10. Wenn du ein Android oder ein Windows Gerät hast ist noch ein weiterer Schritt nötig, um deine email einfach lesen und schreiben zu könnnen.
11. Du musst auf https://account.apple.com/account/manage/section/security erst mal ein app-spezifisches passwort anlegen. Dieses aufschreiben oder anders merken.
12. Dann thunderbird auf android oder windows runterladen. Auf android aus dem play store und auf windows von https://www.thunderbird.net/
13. Nach der Installation musst du folgendes eingeben für IMAP (um email abrufen zu können):
- lina.mueller@icloud.com
- <dein persönliches app passwort>
- imap.mail.me.com
- 993
- ssl/tls
14. Und für SMTP folgendes (um email senden zu können):
- lina.mueller@icloud.com
- <dein persönliches app passwort>
- smtp.mail.me.com
- 587
- starttls
15. jetzt kann beate die dns einträge der domäne so umschiessen, dass die email bei iclud bei den familienmitgliedern landet (details tbd)
16. Solltest du deine email woanders hinleiten wollen (zum beispiel zu gmail) kannst du das selbst unter https://icloud.com/mail einrichten.
17. Um diene alten emails von gmail zu icloud zu übertragen (um zum beispiel nicht mehr bei gmil daüfr bezahlen zu müssen) nutze imap in apple mail oder thunderbird um auf dein altes konto per imap zuzugreifen und übertrage deine alte email in grösseren blöcken vom alten ins neue postfach (details tbd).
18. Falls du dein icloud passwort änderst musst du auch dein app passwort neu erzeugen und eintragen.
