# Voraussetzungen

Voraussetzung sind Kenntnisse für das CMS Contao!

1. Weiterhin sollte ein Startpunkt und eine Seite für die Listenansicht und für die Detailansicht vorhanden sein.
2. Die Contao-Installation muss sich im root-Verzeichnis befinden.
3. jQuery muss bereits eingebunden sein.

# Installation

* 
in das Backend von Contao einloggen
* 
im Menü Backend-Module unter System den Punkt Erweiterungskatalog wählen
* 
im **Suchfeld** „makler modul“ eingeben und die Taste **Enter** drücken
* 
im Suchergebnis rechts oben in der Ecke das **Symbol** zum **Installieren** klicken

ODER

* 
Suchergebnis „makler_modul_mplus“ auswählen und Button **Installieren** klicken
* 
Lizenzschlüssel eingeben und **Weiter**
* 
bei der nächsten Anzeige Aktionszusammmenfassung noch einmal Weiter klicken
* 
wenn Aktion erfolgreich, dann Weiter klicken
* 
Datenbank aktualisieren, zum Abschluss **OK** drücken

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



## 



