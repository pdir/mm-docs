# Dateien für die Immobiliendaten hochladen

Sie haben die Möglichkeit **eigene Immobiliendaten** oder die **Demodaten** zu importieren. 

Wenn Sie zuerst die Demodaten herunterladen wollen, wählen Sie in der linken Navigation unter PDIR APPS den Menüpunkt Maklermodul Setup aus und klicken auf den Button Demodaten herunterladen. Anschließend finden Sie die Demodaten in der Dateiverwaltung unter dem Ordner maklermodul/data.

## Eigene Immobiliendaten importieren

Nach der Installation befinden sich unter Backend-Module **System** im Punkt **Dateiverwaltung** ein neues Verzeichniss  
**maklermodul**. In diesem Ordner müssen **3 weitere Verzeichnisse** mit folgenden Namen  
enthalten sein: **data, org, upload**. Um die zip-Datei hochzuladen, muss auf **Datei-Upload** geklickt werden. Die  
Ansicht ändert sich und es muss rechts von Upload das Icon **In dieses Verzeichnis einfügen** geklickt werden.  
Unter **Dateiupload** den Button **Dateien auswählen** betätigen. Danach die **zip-Datei** wählen und unten  
rechts Button **Öffnen** klicken. Anschliessend den Button **Dateien hochladen** betätigen. Jetzt sollte sich diese  
Datei im **Verzeichnis ‚upload‘** befinden.

## Hinweis

* Unter Backend-Module **System** den Punkt **Einstellungen** wählen und im Bereich **Maximale Upload-Dateigröße** den Wert erhöhen.
* Unter Backend-Module **Layout** den Punkt **Theme** wählen und bei dem angelegten Theme das Icon **Layout ID … bearbeiten klicken** und im Bereich **jQuery laden den **Haken setzen\*\*.
* Wenn Sie das files-Verzeichnis geändert haben, müssen sie über das FTP-Programm unter **system/modules/makler\_modul\_mplus/config** die **import.ini** änderen und das Quell- und Zielverzeichnis ändern. Wenn Sie die dritte Zeile einkommentieren \(Schrägstriche entfernen\), bleibt die Datei nach dem Import erhalten.

## Import starten

Es gibt die Möglichkeit den Import bei dem Backend-Modul **makler modul** über **Tools** und **Import ausführen** manuell auszuführen.

![](importieren-manuell.png)

Oder man kann den Import über den Aufruf folgender URL im Browser ausführen.  
[http://www.ihr-domainname.de/system/modules/makler\_modul\_mplus/assets/cron.php](http://www.ihr-domainname.de/system/modules/makler_modul_mplus/assets/cron.php)

**ihr-domainname** durch **ihre Domain** ersetzen.

Wenn Sie nun die Listenansicht aufrufen, sollte Sie die importierten Objekte aufgelistet sehen. Durch einen Klick auf das Bild eines Objektes gelangen Sie zur Detailansicht.

