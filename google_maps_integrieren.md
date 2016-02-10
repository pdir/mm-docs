# Google Maps integrieren

Zeigen Sie den Standort Ihrer Immobilie in Google Maps. Mit einer einfachen if-Abfrage wird Google Maps nur bei freigegebener Objektadresse geladen. Diese Lösung lädt die Google Maps Karte asynchron, sobald die Seite geladen wurde.

Fügen Sie diesen Code einfach in Ihr eigenes Template "makler_modul_mplus-details.html5" ein.

### Code

```
<!--
  - Google Maps Integration
  - Asynchronous loading
-->
<?php if($this->estate->renderer('verwaltung_objekt.objektadresse_freigeben')->asText()->value(true) == 'true'): ?>

<script>
   var geocoder;
   var map;
   // var address = '<?php $this->estate->renderer('geo.ort')->asText()->value(); ?>'; // Nur den Ort anzeigen
   var address = '<?php $this->estate->renderer('geo.strasse')->asText()->value(); ?> '+
                 '<?php $this->estate->renderer('geo.hausnummer')->asText()->value(); ?>, '+
                 '<?php $this->estate->renderer('geo.plz')->asText()->value(); ?> '+
                 '<?php $this->estate->renderer('geo.ort')->asText()->value(); ?>';
    function initialize() {
       geocoder = new google.maps.Geocoder();
       var mapOptions = {
          zoom: 14,
          center: new google.maps.LatLng( 51.165691 , 10.451526 )
       };
       map = new google.maps.Map(document.getElementById('map-canvas'),mapOptions);
       codeAddress();
    }
		
    function loadScript() {
        var script = document.createElement('script');
        script.type = 'text/javascript';
        script.src = 'https://maps.googleapis.com/maps/api/js?v=3.exp' +
                     '&signed_in=true&callback=initialize';
        document.body.appendChild(script);
    }
		
    function codeAddress() {
       geocoder.geocode( { 'address': address}, function(results, status) {
          if (status == google.maps.GeocoderStatus.OK) {
             map.setCenter(results[0].geometry.location);
             var marker = new google.maps.Marker({
                map: map,
                position: results[0].geometry.location
             });
	  } else {
             // Fehlerbehandlung
             alert('Geocode was not successful for the following reason: ' + status);
	  }
      });
   }
		
    window.onload = loadScript;
</script>
<div id="map-canvas"></div>
<?php endif; ?>
```

### CSS

```
#map-canvas {
 width: 832px;
 height: 400px;
 // weitere Definitionen
}
```

Ein Beispiel der Integration finden Sie hier: [Detailseite mit Google Maps](http://www.maklermodul.de/immobilien/expose/traumhaft-ruhig-wohnen-und-sich-wohlfuehlen.html) 

Stichworte: Immobilien, Maklermodul, Detailansicht, OpenImmo, Kartenanwendung, Maps, XML