# Anpassung der Darstellung

Die Darstellung für Listen- und Detailansicht sind über die Contao Template Engine implementiert. Dies bedeutet, dass Sie wie bei anderen Modulen oder Seitentemplates unter dem Menüpunkt Layout -> Templates unsere Basistemplates duplizieren und dann modifizieren können.

Sofern Sie ein eigenes Template angelegt haben (Empfehlung), können Sie dieses im jeweiligen Modul unter der Einstellung Template auswählen.
Das Template für die Detailansicht bedient sich einer eigens entwickelten API. Deren Dokumentation in der aktuellsten Version finden Sie unter: http://www.maklermodul.de/api-template/

Im Template für die Detailansicht können Sie auf das aktuelle Objekte über $this->estate zugreifen. Dies ist ein Objekt der Klasse FieldRendererFactory: http://www.maklermodul.de/api-template/classes/MaklerModulMplus.FieldRendererFactory.html