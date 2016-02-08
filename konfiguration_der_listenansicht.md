# Konfiguration der Listenansicht

Wie Sie sicher schon bemerkt haben, wurden bei der Einrichtung 2 Felder im Modul **Listenansicht**
ignoriert: **Dargestellte Felder** und **Filter**. Wenn diese beiden Felder leer sind, dann wird die Standardkonfiguration
wirksam, deren Auswirkung Sie aktuell sehen, wenn Sie die Listenansicht aufrufen.

Wie der Name **Dargestellte** Felder bereits andeutet, steuert dieses Eingabefeld, welche Daten in der Listenansicht bereit gestellt werden sollen. Angenommen Sie möchten nur das erste Objektbild zusammen mit dem Titel anzeigen, dann tragen Sie bitte folgendes in das Feld **Dargestellte Felder** ein:

>freitexte.objekttitel<br>
anhaenge.anhang.#1.@gruppe<br>
anhaenge.anhang.#1.daten.pfad<br>
anhaenge.anhang.#1.format<br>
anhaenge.anhang.#1.anhangtitel

**Speichern** Sie die **Einstellungen** des Moduls und rufen Sie folgende **URL** in Ihrem Browser auf: **http://www.ihre-domain.de/system/modules/makler_modul_mplus/assets/indexer.php**.

Wenn Sie nun die Seite mit Ihrer Listenansicht aktualisieren, werden Sie festellen, dass der Filter verschwunden ist. Dies liegt daran, dass die Standardeinstellungen nicht mehr greifen, sobald im Feld Dargestellte Felder etwas eingetragen wurde.

Um Ihren Kunden die Filterung nach Nutzungsart, Vermarktungsart und Ort zu ermöglichen, ergänzen Sie in jeweils beiden Felder folgende Zeilen:

>objektkategorie.nutzungsart.@WAZ<br>
objektkategorie.nutzungsart.@GEWERBE<br>
objektkategorie.nutzungsart.@ANLAGE<br>
objektkategorie.nutzungsart.@WOHNEN<br>
objektkategorie.vermarktungsart.@MIETE_PACHT<br>
objektkategorie.vermarktungsart.@LEASING<br>
objektkategorie.vermarktungsart.@KAUF<br>
objektkategorie.vermarktungsart.@ERBPACHT<br>
geo.plz<br>
geo.ort

**Speichern** Sie die **Einstellungen** des Moduls und rufen Sie folgende **URL** in Ihrem Browser auf: **http://www.ihre-domain.de/system/modules/makler_modul_mplus/assets/indexer.php**.

Nun sollten Sie in der Listenansicht Filter-Buttons für die oben genannten Felder finden. Für jeden Wert der mindestens einmal in einem Objekt vorhanden ist, wird ein Button generiert.

# Sortiermöglichkeiten in der Listenansicht

Sie haben die Möglichkeit Ihre Immobilien in der Listenansicht Ihrer Homepage nach einen bestimmten Feld zu sortieren. Soll keine Sortierung vorgenommen werden, dann stellen Sie es wie im folgenden Bild ein.

![](Sortieren.png)
