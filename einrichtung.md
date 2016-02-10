# Einrichtung

**Hinweis** Wenn Sie das files-Verzeichnis geändert haben, müssen sie über das FTP-Programm unter **system/modules/makler_modul_mplus/config** die **import.ini** änderen und das Quell- und Zielverzeichnis ändern. Wenn Sie die dritte Zeile einkommentieren (Schrägstriche entfernen), bleibt die Datei nach dem Import erhalten.
* 
unter Backend-Module **Layout** den Punkt **Themes** wählen und für das Theme Ihrer Webseite das Icon **Die Frontend-Module des Themes ID … bearbeiten** auswählen
* 
dort **Neues Modul** auswählen – für die Listenansicht
 * Titel für die **Immobilienliste** eingeben und bei Modultyp unter **MaklerModulMplus**
den Eintrag Immobilienliste auswählen
 * bei **Detailansicht** die entsprechende Seite auswählen
 * bei **Immobilien** Templates den Eintrag **makler_list** wählen
 * **Speichern und schliessen** klicken
* 
noch einmal **Neues Modul** auswählen – für die Detailansicht
 * Titel für die Detailansicht eingeben und bei Modultyp unter **MaklerModulMplus**
den Eintrag **Expose** auswählen
 * bei **Immobilien Templates** den Eintrag **makler-details_simple** wählen
 * bei **Immobilienliste** die bereits angelegte Seite, die später die Immobilienliste enthalten soll, auswählen
 * **Speichern und schliessen** klicken
* 
unter Backend-Module **Inhalte** den Punkt **Artikel** wählen und zwei **neue Artikel** für die **Listenansicht** und
**Detailansicht** in den entsprechenden Seiten anlegen und die **neu angelegten Module** einbinden
* 
bei dem jeweiligen Artikel das Icon **Artikel ID … bearbeiten** wählen
 * rechts von den Artikeldaten das Icon n**eues Element oben erstellen** klicken
 * bei Elementtyp den Eintrag „Modul“ wählen
 * die Ansicht ändert sich; bei Modul für die Listenansicht **Listenansicht(ID...)**
und für die Detailansicht **Detailansicht (ID...)** wählen
 * **Speichern und schliessen** klicken



## Dateien für die Immobiliendaten hochladen

Nach der Installation befinden sich unter Backend-Module **System** im Punkt **Dateiverwaltung** ein neues Verzeichniss
**makler_modul_mplus**  . In diesem Ordner müssen **3 weitere Verzeichnisse** mit folgenden Namen
enthalten sein: **data, org, upload**. Um die zip-Datei hochzuladen, muss auf **Datei-Upload** geklickt werden. Die
Ansicht ändert sich und es muss rechts von Upload das Icon **In dieses Verzeichnis einfügen** geklickt werden.
Unter **Dateiupload** den Button **Dateien auswählen** betätigen. Danach die **zip-Datei** wählen und unten
rechts Button **Öffnen** klicken. Anschliessend den Button **Dateien hochladen** betätigen. Jetzt sollte sich diese
Datei im **Verzeichnis ‚upload‘** befinden.

##Hinweis

* Unter Backend-Module **System** den Punkt **Einstellungen** wählen und im Bereich **Maximale Upload-Dateigröße** den Wert erhöhen.
* Unter Backend-Module **Layout** den Punkt **Theme** wählen und bei dem angelegten Theme das Icon **Layout ID … bearbeiten klicken** und im Bereich **jQuery laden den **Haken setzen**.

## Import starten

Es gibt die Möglichkeit den Inde bei dem Backend-Modul **makler modul** über **Tools** und **Import ausführen** manuell auszuführen.

Oder man kann den Import über den Aufruf folgender URL im Browser ausführen.
**http://www.ihr-domainname.de/system/modules/makler_modul_mplus/assets/cron.php**

**ihr-domainname** durch **ihre Domain** ersetzen.

Wenn Sie nun die Listenansicht aufrufen, sollte Sie die importierten Objekte aufgelistet sehen. Durch einen Klick auf das Bild eines Objektes gelangen Sie zur Detailansicht.
