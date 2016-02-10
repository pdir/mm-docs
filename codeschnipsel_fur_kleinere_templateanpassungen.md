# Codeschnipsel für kleinere Templateanpassungen

## Listenansicht

```
Darstellung des Kaufpreis in der Filteranzeige im deutschen Format

jQuery('#estate_list').isotope( 'on', 'layoutComplete', function() {
    jQuery("#estate_filter_list .preise-kaufpreis .button").each(function(i, obj) {
        jQuery(obj).html(filterGermanNumber(jQuery(obj).html()) + ' €');
    });
});
 
//  Hilfsfunktionen
function numberWithPoint(x) {
    return x.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".");
}
function filterGermanNumber(x) {
    var parts = x.toString().split(".");
    parts[0] = parts[0].replace(/\B(?=(\d{3})+(?!\d))/g, ".");
    return parts.join(",");
}
```