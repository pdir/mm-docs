# Sortiermöglichkeiten der Listenansicht

## Sortierung

Sie haben die Möglichkeit Ihre Immobilien in der Listenansicht Ihrer Homepage nach einen bestimmten Feld zu sortieren.

![](Sortieren.png)

Bei **Feldauswahl** können Sie auswählen, nach welchem Feld sortiert werden soll.<br>
Bei **Feldtyp** wählen Sie den Feldtyp (Zahl, Gleitkommazahl oder Text) aus.<br>
Bei **Sortierung** wählen Sie aus ob sie aufsteigend oder absteigend sortieren lassen wollen.

## Bedingungen

![](Bedingungen.png)

Das Feld **Bedingungen** dient zur Reduzierung der Ergebnisse nach bestimmten Kriterien. Wollen Sie z. B. nur Objekte in Leipzig angezeigt haben, können SIe hier folgendes eingeben: **geo.ort=Leipzig** (auf Groß- und Kleinschreibung achten!).

## Bildeinstellungen

![](Bildeinstellungen.png)

Bei **Bildbreite** und **Bildhöhe** gibt man eine Angabe der Breite bzw. der Höhe in Pixel an. Standards sind für die Breite 293px, für die Höhe 220px.

**Bildmodus** gibt an wie das Bild in der Listenansicht an die entsprechende Bildbreite und -höhe skaliert wird. Folgende Angaben sind möglich:
* 
**proportional:** 
* 
**box:**
* 
**crop:**
* 
**left_top:** linker oberer Bildausschnitt
* 
**center_top:** mittige obere Bildausschnitt
* 
**right_top:** rechte obere Bildausschnitt
* 
**left_center:** linke mittige Bildausschnitt
* 
**center_center:** mittige Bildausschnitt
* 
**right_center:** rechte mittige Bildausschnitt
* 
**left_bottom:** linke untere Bildausschnitt
* 
**center_bottom:** mittige untere Bildausschnitt
* 
**right_bottom:** rechte untere Bildausschnitt



## Paginierung

![](Paginierung2.png)

Bei **Anzahl der Objekte** kann man auswählen, wie viele Objekte auf einer Seite angezeigt werden sollen.

Bei **Anzahl der Links** kann man auswählen wie viele Links man in der Seitennummerierung (siehe folgendes Bild) angezeigt haben möchte. Wenn man z. B. 2 einträgt, werden im nachfolgenden Bild nur die 2 und 3 angezeigt. Die restlichen Nummern werden dann mit ... angezeigt.

![](pagination-anzahl-der-links.png)

**Verwende Isotope** bewirkt, dass die Elemente sich verschieben, wenn man Filter anwendet.

## Optionen

![](Optionen.png)

**Nur Filter** blendet alle Filterergebnisse aus. Wenn diese Option aktiv ist, muss bei **Listenansicht** eine Seite angegeben werden auf die weitergeleitet wird, die die Filtereinstellungen mit übernimmt.

Bei **In Sitemap-Navigation anzeigen** werden die Objekte dieser Listenansicht auch in der Sitemap Navigation angezeigt. Es muss das Template "nav_makler-sitemap" in den Templateeinstellungen der Sitemap-Navigation ausgewählt werden.

**Debug** zeigt alle verfügbaren Feldschlüssel an, die verwendet werden können.

**CSS einbinden** bindet das moduleigene CSS in das Template ein.

**Javascript einbinden** bindet das moduleigene Javascript ind as Template ein.

**Abwärtskompatibilität** aktivieren bedeutet, dass nach Aktivierung die alten Template-Funktionen in der Listenansicht verwendet werden (frühere Versionen <1.4.0). Der Index muss nach einer Änderung neu aufgebaut werden.