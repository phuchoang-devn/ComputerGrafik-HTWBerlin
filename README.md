# Computer Grafik | Final Project | Medieninformatik SS23 | HTW Berlin 

## Beschreibung des Projekts:
Unser Projekt handelt von einem verlassenen Raum in Ägypten, in dem sich der Pharao in der Mitte zusammen mit ägyptischen Schriftzeichen und Hieroglyphen an der Wand befindet.
Es geht darum, dass eine Person mit einer Taschenlampe (da es keine Beleuchtung gibt) ängstlich in den Raum geht. Ihre aufgeregte Atmung ist durch das ständige Auf und Ab des Taschenlampenlichts zu erkennen. Durch Klicken mit der Maus kann die Person die Taschenlampe in jede gewünschte Richtung lenken.
Durch das Fenster sind Bäume zu sehen, und in regelmäßigen Abständen erscheinen Blitze während des Sturms.

Die Arbeit wurde von Martin Bonhomme und Anh Phuc Hoang für das Fach Computergrafik im dritten Semester des Bachelor-Studiengangs Medieninformatik durchgeführt.

### Technischen Herausforderungen:
* Platzierung der Wände, Decke und Boden des Raumes: Anfangs platzierten wir die Wände als Würfel, der sich überlappte, was zu seltsamen Schatten führte. Daher änderten wir es, so dass die Seiten des Würfels nur über eine Kante miteinander verbunden sind. Im Bild ist dies besser zu erkennen:
![WhatsApp Image 2023-07-05 at 09 23 36](https://github.com/mar7-n/Final-Project--Computer-Grafik--SS23/assets/116806411/8efa758d-1574-4a5d-9d62-e8fe0971bbe3)
* Maße des Raums: Anfangs wussten wir nicht genau, welche Maße wir für den Raum verwenden wollten. Daher entschieden wir uns für eine generische Lösung, basierend auf Variablen, die die Maße der Wände enthielten. Dadurch mussten wir bei einer späteren Änderung der Maße nicht den gesamten Code ändern, sondern nur den Wert der Konstanten anpassen.
* Fenster: Bei der Erstellung der Fenster hatten wir Schwierigkeiten, da wir nicht wussten, wie man ein Loch in einem Objekt erstellt. Nach Recherchen fanden wir heraus, dass Boolean-Operationen zwischen Objekten verwendet werden können, um das Loch zu erstellen. Dafür müssten wir jedoch "threecsg.js" verwenden, dessen Dokumentation in einem anderen Repository lag. Wir waren uns nicht sicher, ob wir es in unserer Arbeit verwenden durften. Daher entschieden wir uns für einen weniger praktischen Ansatz, bei dem wir die Wand in 4 Wände aufteilten und das Fensterloch an der Verbindung zwischen ihnen bildeten. Dies zusammen mit der Implementierung der generischen Maße der Wände verlangsamte die Arbeit erheblich.
* Spiegel: Die Hinzufügung des Spiegels auf dem Pharao war ebenfalls eine Herausforderung, da die Zugabe eines Spiegel-Objekts allein nicht ausreichte, da das Bild nicht reflektiert würde. Schließlich implementierten wir es mit dem Element "Reflector", aber die Reflexion war aufgrund des Mangels an Licht nicht gut sichtbar. Daher fügten wir eine weitere Lichtquelle in der Szene hinzu, um den Spiegel zu beleuchten.
* Camera: Am Anfang haben wir Orbitscamera ausgesucht. Wir habe auch sehr viel eingestellt, aber für einen 1. person view passt es gar nicht... oder haben wir nicht richtig gemacht. Und am Ende haben wir selbst die Bewegung für den Camera aufgebaut (mit Group).
* Background: es sah nicht so wie in der Realität aus, wenn wir den Background mit einem gruseligen Bild versah. Am Enden haben wir es mit einer Farbe gemalt und das Moonlicht hinzugefügt, damit es bisschen wie in der Nacht aussieht. 
