Maps Example for Android
====

Maps (Google, Bing, Here, Leaflet)

Dies ist eine kleine Zusammenstellung der Vier oben genannten Maps-Anbieter.
Weitere Details dazu auf deren Webseiten.

##### here
http://developer.here.com/javascript-apis/documentation/maps/topics/overview.html
Dies ist wohl die einfachste Art eine Map zu integrieren. Einfach Konto auf https://developer.here.com/ einrichten und mit APP ID und TOKEN https://developer.here.com/javascript-apis/documentation/maps/topics/quick-start.html sofort durchstarten. 
##### leaflet
http://leafletjs.com/index.html
Mit dieser API ist es möglich gänzlich ohne Authentifizierung zu arbeiten. Die Nutzung in meinem Beispiel harkt aber noch etwas.
##### bing
https://code.google.com/p/jquery-bing-maps/
Es gibt eine Trail Version, das ganze scheint aber nicht kostenlos. Das anlegen und verwalten ist zunächst am umfangreichsten http://msdn.microsoft.com/en-us/library/ff428642.aspx aber einmal eingerichtet ist die Anbindung ein Kinderspiel. https://www.bingmapsportal.com/application/index/ Mein Key läuft am Expiration Date: 05/27/2014 ab.
##### google
https://developers.google.com/maps/documentation/javascript/examples/?hl=de-DE
Für die Nutzung der API aus einer Webview im Browser oder einer APP auf HTML Basis ist der Key scheinbar nicht zwingend notwendig. Ich jedenfalls habe ein positives Ergebnis ohne und in jeglichen Konstellationen für einen Browser-Key mit Referers *.* oder * werden meine Requests nicht akzeptiert https://console.developers.google.com/project/apps~webrtc42/apiui/credential.
##### Die Erkentnisse aus dem APP build findet ihr hier
http://mitchobrian.github.io/ConactsList/
##### Geolocation
Beim ersten mal kein triviales Thema. Wichtig bei der Erstellung einer APP auf HTML Basis ist die richtige Einstellung der nativen Parameter. Für Android auf keinen Fall das Manifest vergessen.
http://docs.phonegap.com/en/1.8.0/cordova_geolocation_geolocation.md.html
Viele Probleme bei der Entwicklung treten dann auf, wenn man selber einmal im Browser das lesen der Position verbietet. Dazu gibt es bislang wohl auch kein Heilmittel. Stack Overfow ist voll davon https://support.google.com/gmm/answer/1250068?hl=en Sind die Einstellungen frisch sollte es mit einem einfachen Beispiel reibungslos funktionieren http://www.w3schools.com/html/html5_geolocation.asp – https://developer.mozilla.org/en-US/docs/WebAPI/Using_geolocation.