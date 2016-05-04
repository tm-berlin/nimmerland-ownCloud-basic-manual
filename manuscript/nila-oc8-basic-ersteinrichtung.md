# Hallo!

Schön, dass du dich für **nimmerland ownCloud basic** entschieden hast. 'basic' ist unser preiswerter Tarif für den persönlichen Gebrauch. Wie bei Dropbox oder Google Drive hast bekommst du bei uns Speicherplatz für deine privaten Dateien und Bilder. Zusätzlich kannst Du ein Adressbuch und einen Kalender anlegen und alles mit all Deinen Geräten synchronisieren.

Deine Daten und die Backups liegen sicherer[^1] in einem Berliner Rechenzentrum. Daher gelten die strengen europäischen Datenschutzregeln. Unsere Server werden mit Naturstrom betrieben.

[^1]: sicherer. Denn ganz sicher gibt es nicht. Gestern sicher geglaubtes gilt heute als zweifelhaft oder muss überprüft werden. Wir tun unser Bestes. Willst du mehr über [Netzpolitik](https://netzpolitik.org/) wissen oder aktuelle [Informationen über Sicherheit im Netz](http://www.heise.de/security/) erhalten? Nutze die Links.

Du bist jetzt bereit, selbst die Kontrolle über deine persönlichen Daten zu übernehmen. Wir helfen Dir mit dieser Anleitung zur Ersteinrichtung.

# Die nimmerland ownCloud

Deine nimmerland ownCloud basic ist ein persönlicher Bereich auf cloud.nimmerland.de. Im Unterschied zu unseren anderen Tarifen ist dein Bereich nicht als eigene ownCloud Server Instanz realisiert (genau wie bei dropbox, google drive und anderen). cloud.nimmerland.de wird von unseren Technikern administriert. Du brauchst dich nicht um Updates kümmern.

![](media/image3.png)

1.  Sicherheit

    1.  Transportverschlüsselung (https/ssl)

Auf dem Weg durch das Internet sind deine Daten verschlüsselt. Wir nutzen Class 2 Wildcard Zertifikate von StartCom. Du kennst das von deinen Bankgeschäften: ein Schloss in der Adressleiste deines Browsers zeigt dir eine verschlüsselte Verbindung an. Du kannst auf das Schloss klicken, um genaueres über die Verschlüsselung zu erfahren.

![](media/image4.png)

[SSLLabs](https://www.ssllabs.com/ssltest/analyze.html?d=cloud.nimmerland.de&latest) bewertet die Sicherheit unseres Services zur Zeit mit 'A'.

## Serverseitige Verschlüsselung (ownCloud)

Auf unseren 'basic'-Installationen haben wir das Server-Side-Encryption-Modul aktiviert. Alle Dateien in deiner Cloud werden vom nimmerland ownCloud-Server verschlüsselt. Weil die Schlüssel mit den Dateien auf dem Server liegen gilt dieses Verfahren nicht als 100%ig sicher.

## Clientseitige Verschlüsselung (Boxcryptor & Co.)

Deine Daten sind dann bestens vor fremden Blicken geschützt, wenn sie lokal auf deinen Geräten verschlüsselt werden bevor sie in deine nimmerland ownCloud hochgeladen werden. Die Schlüssel bleiben auf deinem Rechner. Zwei deutsche Firmen bieten gut getestete Software dazu an: [Boxcryptor](https://www.boxcryptor.com/) wird kontinuierlich weiterentwickelt und bietet Clients für alle Betriebssysteme und mobilen Geräte. Boxcryptor hat erlaubt Zugriffsrechte nach Ordnern, Benutzern oder Gruppen differenziert zu vergeben und eignet sich daher besonders für Teams und kleine Firmen. Eine sehr eingeschränkte Version ist für den Privatanwender kostenlos.

Ähnlich und für Privatabwender in einem weiteren Umfang kostenlos ist [Cloudfogger,](https://www.cloudfogger.com/de/) ebenfalls eine deutsche Software. Die mobilen Clients von lassen allerdings nur das Entschlüsseln, nicht das Verschlüsseln von Dateien zu. Wenn du einen Text auf deinem Tablet schreibst und ihn direkt in deiner ownCloud speicherst, wird Cloudfogger ihn nicht verschlüsseln. Wer mobil überwiegend lesend auf seine Daten zugreift und keine fein differenzierten Zugriffsrechte benötigt, ist mit Cloudfogger gut bedient.

Seit März 2015 gibt es die Software [Panbox](http://www.sirrix.de/content/pages/Panbox.htm), die von der Fa. Sirrix AG im Zusammenarbeit mit dem [Fraunhoferinstitut](https://www.sit.fraunhofer.de/de/panbox/) entwickelt wurde. Sie soll vielen Menschen kostenlose und einfache Verschlüsselung bieten. Die Besonderheit gegenüber den beiden vorherigen Lösungen ist, dass Schlüssel nicht über den Server eines Anbieters ausgetauscht werden. Stand 03/2015 gibt es die Software allerdings nur für Windows und Android und die Installation ist noch nicht wirklich benutzerfreundlich.

Für wirklich sensible Daten empfehlen wir dir eine clientseitige Verschlüsselung. Auch wenn die Bequemlichkeit der Nutzung etwas leidet: Dateien müssen immer zweifach geteilt werden: einmal die Zugriffsrechte (ownCloud) und einmal die Entschlüsselungsrechte (z. B. Boxcryptor)

# Zugangsdaten

Dein Passwort bekommst du per SMS. Benutze immer sichere Passwörter und bewahre sie gut auf. *Hier erfährst du, wie du ein sicheres Passwort erstellst …*

**Tipp!!! Wenn du Dein Passwort ändern willst, tu es bevor du Daten in deiner Cloud speicherst. Andernfalls müssen all deine Dateien mit einem neuen Schlüssel versehen werden, was ein Zeitlang dauert und auch zu Datenverlust führen kann.**

# ownCloud Apps

Die ownCloud-Software ist modular aufgebaut. Apps können im Menü sichtbar sein oder im Hintergrund ihren Dienst verrichten. Folgende Apps haben wir für dich geprüft und aktiviert.

## Activity

Der Activity-Feed führt Protokoll über deine Aktivitäten. Du kannst nachvollziehen, wann und mit wem du eine Datei geteilt hast, sie bearbeitet oder gelöscht hast.

![](media/image5.png)

## Bilder / Galerie

Dein Fotoalbum. Du kannst Alben (Ordner) teilen. JPGs und PNGs können als selbstablaufende Diashow angesehen werden. Die App ist standardmäßig aktiviert.

**Info!!! Das ownCloud Team arbeitet an einer neuen Bildergalerie (gallery+), die erweiterte Möglichkeiten zum Teilen von Bildern hat und auch einige RAW- und Tiff-Dateien anzeigen kann. Wenn das Modul hinreichend getestet ist, werden wir es dir zur Verfügung stellen.**

## Bookmarks

Deine eigene Lesezeichenverwaltung. Lesezeichen (und damit ein Abbild deiner Interessen) werden nur in deiner eigenen Cloud und nicht auf dem Server eines Browserherstellers, bzw. auf den Servern von Apple oder Google gespeichert. Zur Zeit gibt es keine Synchronisation mit Browsern, jedoch Plugins, Snippets und mobile Apps mit denen du auf deine ownCloud-Lesezeichen zugreifen kannst.

## Calendars

Deine ownCloud Terminverwaltung. Du kannst mehrere Kalender anlegen und sie mit anderen telen. Du kannst auch einzelne Termine mit anderen teilen. Selbstverständlich kannst du Deine Kalender mit deinem Mailprogramm (Outlook braucht allerdings ein besonders Plugin, z.B. [cFos Outlook DAV](http://www.cfos.de/de/download/download.htm?__ntrack_pv=1)) und mit deinen mobilen Geräten synchronisieren.

Der Superadministrator muss diese App aktivieren, sie ist standardmäßig nicht aktiviert.

## Contacts

Deine ownCloud Adressverwaltung. Du kannst Adressbücher anlegen und mit anderen teilen. Über das Caldav-Protokoll kannst du deine Kontakte mit vielen Mailprogrammen, und allen mobilen Plattformen synchronisieren.

## Files Move

Der Name ist Programm: Diese kleine App erlaubt es Dateien einfacher zwischen Ordnern zu verschieben.

![](media/image6.png)

**Info!!! Alternativ installieren wir in einigen Installationen eine Clipboard-App.** 

Der Superadministrator muss diese App aktivieren, sie ist standardmäßig nicht aktiviert.

## News

Dein Feed-Reader. Du kannst das Web-Interface oder eine Android-App nutzen um deine News zu lesen. Die Adressen deiner Feeds (und damit ein Abbild deiner Interessen) werden nur in deiner eigenen nimmerland ownCloud und nicht auf fremden Servern gespeichert.

## PDF

Du kannst deine PDF gleich online ansehen. Herunterladen ist nicht nötig. Diese App ist per default aktiviert.

## Server-Side Encryption

Die serverseitige Verschlüsselung ist eingeschaltet. Daher bedeutet ein Verlust des Passwortes in der Regel auch einen Verlust der Lesbarkeit deiner Daten.

**Bitte setze Dein Passwort nicht selbst zurück!** Wir können Dir ein neues Passwort zuweisen, wenn du **vorher** in deinen persönlichen Einstellungen **die Passwort-Wiederherstellung aktiviert hast.** 

Der Administrator kann in keinem Fall die Dateien lesen. Selbst wenn sie oder er die Verschlüsselung abschalten sollte, kann nur der Benutzer die Dateien entschlüsseln.

1.  Ersteinrichtung

    1.  Einloggen

Logge dich zuerst als Superadministrator mit deinem 12-stelligen Passwort ein.

![](media/image3.png)

Wenn du dich zum ersten Mal einloggst, hilft Dir ein Assistent dabei deinen Computer und dein mobiles Gerät mit deiner Cloud zu verbinden, sodass du deine Daten jederzeit und überall synchron halten kannst.

![](media/image7.png)

Du musst das nicht gleich tun, du kannst den Assistenten jederzeit wieder aufrufen.

Weitere Hilfe findest du auf unserer Webseite: [nimmerland.de/anleitungen.html](https://nimmerland.de/anleitungen.html)

## Persönliche Einstellungen

![](media/image8.png)

Auf der rechten Seite kommst du zu deinen persönlichen Einstellungen.

### Freier Speicherplatz

Hier oben siehst du, wie viel Speicherplatz deine Dateien von dem Kontingent belegen, dass dir der Superadministrator zugewiesen hat. Für diese Anzeige werden lediglich die Dateigrößen addiert. Wenn du sehr viele kleine Dateien gespeichert oder viele Ordner in deiner Cloud angelegt hast, kann es vorkommen, dass du deinen Speicherplatz überschreitest, obwohl hier noch alles in Ordnung scheint.

**nimmerland garantiert dir je 5GB mindestens 5000 Dateien oder 500 Ordner.** Wir melden uns bei dir, wenn dein Kontingent erschöpft ist, du kannst dann entweder Dateien löschen, den Papierkorb leeren oder eine Speichererweiterung kaufen.

![](media/image9.png)

### Vollständiger Name

Diesen Namen, den deine Freunde sehen, mit denen du Dateien teilst, kannst du ändern. Dein **Benutzername,** den du zum Einloggen benutzt, ist unveränderlich.

### E-Mail

Du kannst dich automatisch benachrichtigen lassen, falls eine Datei oder einen Ordner mit dir geteilt wird, wenn du hier deine E-Mailadresse einträgst. Wir von nimmerland.de erfahren diese Adresse nicht und benutzen sie auch nicht für den Kontakt mit dir.

## Sprache

Wähle die Sprache deiner nimmerland ownCloud-Oberfläche. Wenn du einen Fehler findest, kannst du bei der Übersetzung helfen.

## Benachrichtigungen

Benachrichtigungen kannst du per Mail oder im Activity-Stream bekommen. Den Stream kannst du auf der Weboberfläche ansehen (Modul Activity) oder als RSS-Feed abonnieren. Hier wählst du aus, worüber du auf welcher Weise informiert werden möchtest.

1.  Benutze deine Cloud

    1.  Hilfen & Anleitungen

Auf der Weboberfläche Deiner nimmerland ownCloud findest du eine Hilfe in deutscher Übersetzung. Du findest sie nach dem Login im Drop-Down-Menü unter deinem Namen. Hier findest du auch Links zu ownCoud-Community. Gerade bei speziellen Problemen hilft ein Blick in die Foren.

Die aktuelle englischsprachige Hilfe zu [ownCloud-Server](https://doc.owncloud.org/server/8.0/user_manual/) und dem [ownCloud Desktop-Client](https://doc.owncloud.org/desktop/1.8/) findest du [hier](http://doc.owncloud.org/).

Auf unserer Webseite findest du ein paar deutschsprachige [Anleitungen](https://nimmerland.de/anleitungen.html) zur Arbeit mit bestimmten Modulen verlinkt.

## Kalender & Kontakte

Wie du Deinen Kalender und Deine Kontakte mit deinen Mailprogrammen und mobilen Geräten synchronisierst, erfährst du in der Hilfe. Ein paar deutschsprachige Anleitungen sind auf unserer [Webseite](https://nimmerland.de/anleitungen.html) verlinkt. Du kannst auch [DuckDuckGo](https://duckduckgo.com/) fragen.

### Empfohlene Apps

[Thunderbird](https://www.mozilla.org/de/thunderbird/) mit [Lightning](https://addons.mozilla.org/de/thunderbird/addon/lightning/) und [Enigmail](https://addons.mozilla.org/de/thunderbird/addon/enigmail/)

[eM Client](http://de.emclient.com/) (bietet Verschlüsselung mit s/mime)

[CardDAV-Sync](http://dmfs.org/carddav/) und [CalDAV-Sync](http://dmfs.org/caldav/) für die Synchronisation mit Android-Smartphones (arbeitet gut mit selbst signierten Zertifikaten zusammen)

## Dateien und Galerien teilen

Deine nimmerland ownCloud 8 bietet vielfältige Möglichkeiten Dateien und auch Fotogalerien mit Freunden und Familie zu teilen. Ausführliche Hinweise dazu findest du in den Hilfen. Achte selbst auf deine Sicherheit. Teile nur mit Passwort achte darauf, wem du Zugriff auf deine Dateien gewähren möchtest. Du kannst den Dateizugriff auch zeitlich beschränken.

## Dateien synchronisieren

Es gibt [Desktop-Clients](https://owncloud.org/install/#install-clients) für alle bekannten Betriebssysteme. Die Clients betreiben einigen Aufwand auf allen synchronisierten Rechnern immer die aktuelle Version einer Datei vorzuhalten. Das braucht Zeit und läuft auch nicht immer einwandfrei.

### Desktop Client einrichten

Der Desktop-Client synchronisiert einzelne Ordner deiner nimmerland ownCloud mit deinem lokalen Rechner. Du kannst den passenden Client für dein Betriebssystem kostenlos bei [owncloud.org](https://owncloud.org/install/) herunter laden und installieren.

### Zugangsdaten eingeben

Rufe den Verbindungsassistenten auf und gib die URL deiner nimmerland ownCloud und deine Zugangsdaten ein.

![](media/image10.png)

Die Transportverschlüsselung ist dauerhaft eingeschaltet.

![](media/image11.png)

### Wähle deinen lokalen Synchronisations-Ordner

Seit der Desktop-Client Version 1.7 kannst du die Ordner in der Cloud auswählen, die mit deinem lokalen Computer synchronisiert werden sollen.

![](media/image12.png)

Du kannst die ausgewählten Ordner jederzeit in den Client-Einstellungen ändern.

![](media/image13.png)

Fertig! Sobald du auf 'Verbinden' klickst beginnt der Client mit der Synchronisation.

![](media/image14.png)

Nach erfolgreichem Start zieht sich der ownCloud Desktop-Client in den Systemtray (Windows) oder die obere Mitteilungsleiste (Mac) zurück. Du erkennst ihn am kleinen blauen ownCloud-Symbol und kannst ihn von dort jederzeit aufrufen und Einstellungen ändern.

![](media/image15.png)

### Empfohlene Apps

[ownCloud Desktop-Client](https://owncloud.org/install/#install-clients) (aktualisiere den Client regelmässig)

[Folder Sync](http://www.tacit.dk/foldersync) ist eine Alternative für die Synchronisation mit deinen Android-Geräten. Die Software hat einen etwas anderen Ansatz als die ownCloud Software und lässt sich sehr genau konfigurieren.

## Die Synchronisation

Der Abgleich von Änderungen an deinen Dateien braucht Zeit. Der Dateiupload ist bei den meisten Internet-Anschlüssen wesentliche langsamer als der Download. Der Synchronisations-Client hält sich im Hintergrund und nutzt Zeiten in denen du das Netz nicht für andere Zwecke brauchst.

![](media/image16.png)

Den Verlauf des Dateiuploads kannst du im Activity-Report des Clients verfolgen. Fehler erkennst du an dem roten 'X'. Bei schlechten Internet-Verbindungen kann es vorkommen, das Dateien bei wiederholten Fehlern von der Synchronisation ausgeschlossen werden (blacklisted). Du kannst die Synchronisation dann manuell wieder anschieben (Datei anwählen → 'Synchronisation wiederholen')

## Papierkorb und Versionierung

Deine nimmerland ownCloud arbeitet intern mit einem Papierkorb und Versionierung. Für jede gelöschte oder geänderte Datei werden Kopien in der Cloud gespeichert. Maximal verwendet ownCloud 50% deines Speicherplatzes für diese Dateien.

Zugriff auf alte Versionen oder gelöschte hast du nur über die Webschnittstelle. Hier kannst du sie wieder herstellen.

**Tipp!!! Falls wir dich bitten, deinen Speicherplatz zu überprüfen, weil du dein Kontingent überschritten hast, schau zuerst nach ob du auf Versionen verzichten und/oder deinen Papierkorb leeren kannst.**

## Web-Interface kennenlernen

Über die Webschnittstelle kannst du dein persönliches nimmerland ownCloud Passwort ändern, im Activity-Log sehen, was mit deinen oder den mit dir geteilten Dateien geschehen ist oder eine einzelne Datei herunter laden. Wenn du hier deine E-Mailadresse hinterlässt, wirst du von der Cloud über Neuigkeiten informiert. Du kannst für verschiedene Ereignisse einstellen, ob du per Mail oder lediglich über die Activity-Application informiert werden möchtest.

### Gelöschte Dateien

Werden je nach verfügbarem Speicher bis zu 30 Tagen aufbewahrt. Du findest nur Dateien im Papierkorb, die du selbst gelöscht hast. Nicht von dir selbst gelöschte Dateien – falls du einen Ordner geteilt hast – kann der Administrator wieder herstellen.

TIPP!!! Wenn du auf geteilte Dateien zugreifst, und eine Datei vermisst, schau im Activity-Stream, wer die Datei gelöscht hat und bitte ihn die Datei wieder herzustellen.

![](media/image17.png)

ACHTUNG!!! Wenn du clientseitige Verschlüsselung mit Boxcryptor benutzt, kannst du deine Dateien oder Bilder online nicht ansehen. Du musst sie downloaden und mit der Boxcryptor-Software entschlüsseln oder – bei wiederhergestellten Dateien – die Synchronisation abwarten und sie über das Boxcryptor-Laufwerk öffnen.Datei-Versionen

nimmerland ownCloud speichert regelmäßig Versionen der von dir benutzten Dateien. Welche es zu einer bestimmten Datei gibt, klärt ein Klick auf den Eintrag 'Versionen'.

![](media/image18.png)

### Activity

Der Activity-Feed führt Protokoll über deine Aktivitäten und die deiner Nutzer. Du kannst nachvollziehen, wann und mit wem du eine Datei geteilt hast, sie bearbeitet oder gelöscht hast.

![](media/image5.png)

**Tipp!!! Falls du gewohnt bist mit RSS-Readern zu arbeiten, kannst du die Neuigkeiten auch als Feed abonnieren.**

1.  Tipps und Hints zum Desktop-Client

    1.  Datei- und Ordnernamen

Ein leidiges Thema: Cloud-Dateien liegen auf unterschiedlichen Rechnern oder mobilen Geräten mit unterschiedlichen Betriebs- und Dateisystemen. Nicht alle halten sich an den globalen Standard UTF-8. Es mag alles glatt gehen, besser ist: Keine Leerzeichen, Sonderzeichen oder Umlaute in Datei- und Ordnernamen.

### Löschen großer Datenmengen

ownCloud Server löscht Dateien nicht, sondern kopiert sie in einen Papierkorb, damit du sie bei Bedarf wieder herstellen kannst. (siehe Geduld)

### Synchronisation mehrerer Geräte

Läuft problemlos, wenn die Uhren in etwa gleich gestellt sind. **Nach der Erstinstallation aber, solltest du erst ein Gerät und dann streng nacheinander alle weiteren Geräte synchronisieren.** Es kann sonst vorkommen, das die Clients gegeneinander arbeiten und gerade hoch geladene Dateien wieder verschwinden.

### Geduld

Du kannst flüssig mit deinen Daten arbeiten. Die Synchronisation über das Netz brauch aber Zeit. Gerade bei großen Datenmengen. Gib der Migration etwas Zeit. Wenn nach einer Woche immer noch Fehlermeldungen kommen, melde dich bei uns.

### Synchronisationsfehler

Können unterschiedliche Ursachen haben. Oft ist eine instabile oder schwache Internetverbindung schuld, gerade wenn sehr große Dateien synchronisiert werden sollen. Damit zumindest die kleineren Dateien aktualisiert werden, blacklistet der Client Files mit mehr als drei gescheiterten Synchronisationsversuchen: Er schließt sie von der zukünftigen Synchronisation aus. Der Activity-Report deines Clients zeigt eine Fehlermeldung.

![](media/image19.png)

Um eine ausgeschlossen Datei wieder zu synchronisieren, aktivierst du sie und klickst 'Synchronisation wiederholen.

![](media/image20.png)

Vielleicht siehst du einmal die Meldung 'Datei wurde nicht synchronisiert, weil sie auf der Ignorierliste geführt ist'. Hierbei handelt es sich meist um versteckte oder Systemdateien, die nicht synchronisiert werden sollen.

1.  Bekannte Probleme

    1.  Umbenennen größerer Ordnerstukturen

Der alte Ordnername ist für die Cloud gelöscht. Daher werden ggf. Unmengen Daten in den internen Papierkorb verschoben. Was Zeit braucht. Zeitgleich wird der umbenannte Ordner neu hochgeladen. Auf anderen synchronisierenden Clients wird eine wahre Löschorgie in Gang gesetzt und man meint die Dateien würden von der Cloud gelöscht. (Panik macht sich breit).

Zwar ist – wenn man nicht eingreift – nach ein paar Stunden wieder alles OK, besser vermeiden oder über das Web-Interface umbenennen.

### Umlaute, Sonderzeichen in Datei/Ordnernamen (Mac)

ownCloud benutzt den UTF-8 Standard um mit allen möglichen Zeichensätzen konsistent umgehen zu können. Einige MAC-User berichten über das Verschwinden von Dateien beim Umbenennen, wenn diese Umlaute enthalten. Möglicherweise ist auf diesen Mac-System der UTF-8 Zeichensatz nicht als Standard gesetzt. Die Dateien sind dann im Papierkorb zu finden.

## nimmerland ownCloud als Laufwerk einbinden

Grundsätzlich kannst du deine Cloud auf allen Betriebssystemen als Laufwerk einbinden. So kannst du – solange du online bist – auch ohne Synchronisation auf deine Dateien zugreifen. Das funktioniert problemlos mit Apple- und Linux- Rechnern. Windows hat leider Probleme mit der starken Transportverschlüsselung (https/ssl). Anleitungen für dein Betriebssystem findest du im Netz.

### Empfohlene Apps

Mac- und Linux- User brauchen keine zusätzliche Software.

[Netdrive](http://www.netdrive.net/) bringt deine Cloud als Netzlaufwerk auf deinen Windows-Rechner. Die Vollversion kostet nach 30 Probetagen 40\$ pro Rechner. Sie bietet Konfigurationen für viele große Cloudanbieter mit. Nach Ablauf der Testphase kannst du nur noch eine Cloud einbinden und musst bei jedem Start der Software die Verbindung selbst herstellen. Für deine nimmerland ownCloud kann das reichen.

[Cyberduck](https://cyberduck.io/index.de.html?l=de) ist eine WebDav-Client, der dir komfortablen Zugriff auf viele Clouddienste ermöglicht, sich aber nicht in das Windows Dateisystem integriert. Cyperduck kannst du gegen eine Spende nutzen. Cyperduck erlaubt neben dem direkten Zugriff auch die Synchronisation einzelner Ordner.

[FX File Explorer](https://play.google.com/store/apps/details?id=nextapp.fx&hl=de) ist ein sehr umfangreicher Filebrowser für dein Android-Gerät, der dir unter 'Network' ebenfalls eine stabile WebDav-Verbindung in deine Cloud ermöglicht.

# Service und so weiter

Um vielen da draußen einen guten sicheren Service zu bieten, kostet nimmerland-cloud basic wenig Geld. Damit das funktioniert, darf es uns auch fast keine zusätzliche Arbeit machen. Natürlich helfe wir dir bei Fragen gern. Bevor du schreibst, schau bitte selbst im FAQ, im ownCloud-Forum oder bei [DuckDuckGo](https://duckduckgo.com/), ob du eine Lösung für dein Problem findest.

Deine nimmerland ownCloud für deine Kontakte, Termine, Bilder und Dokumente kannst du ab jetzt ein Jahr lang nutzen. Etwa vier Wochen vor Ablauf werden wir dir eine Rechnung mit Paypal-Link per E-Mail senden, mit der du deinen Account um ein weiteres Jahr verlängern kannst. Wenn du nicht verlängern möchtest, zahlst du einfach nicht. Dein Account und auch deine Daten werden dann zum Stichtag gelöscht.

# Nutzungsbedingungen & Haftung

nimmerland ownCloud basic wendet sich an Privatanwender. Wir tun alles für einen stabilen Service und geschmeidige Nutzung können dir aber keine ungestörte Verfügbarkeit deiner Daten garantieren. Auch wenn wir ein nächtliches Backup durchführen, liegt es in deiner Verantwortung deine Daten zu sichern. Für direkte und indirekte Schäden, die sich aus der Nutzung unserer Dienste ergeben und dem eventuellen Verlust deiner Daten ergeben, können wir nicht haften. Wir schließen das ausdrücklich aus.

Wir stellen Dir eine Cloud für deine persönliche Nutzung zur Verfügung. Wir erlauben dir nicht, Teile deines Speicherplatzes gegen Entgelt Anderen zu überlassen. Wir erwarten, dass du dich beim Teilen von Dateien an geltendes Recht hältst und unter keinen Umständen pornografisches, volksverhetzende und zur Gewalt aufrufendes Material in deiner Cloud teilst.

Den genauen Wortlaut unserer [Nutzungsbedingungen, AGB](https://nimmerland.de/agb.html) und unsere [Datenschutzerklärung](https://nimmerland.de/impressum.html) findest du in der jeweils aktuellen Fassung jederzeit auf unserer Webseite.

# Herzlichen Glückwunsch

Du hast deine nimmerland ownCloud eingerichtet. Wir wünschen dir viel Spaß beim Entdecken deiner neuen Möglichkeiten.

Beste Grüße aus Berlin, Thomas Michalak
