# Stundenprotokoll - Informatikprojekt: Audio Spectrum Analyzer (Lukas u. Torben)
<br>

## Vorwort
In diesem Repository haben wir alle Inhalte der Unterrichtsstunden und privaten Treffen im Rahmen unseres ersten Informatikprojekts notiert. Das Produkt des Projekts ist ein Audio Spectrum Analyser, ein Gerät, welches die Präsens und Stärke verschiedener Frequenzen in Musik, beispielsweise vom Handy, darstellt. Mehr Informationen zum Audio Spectrum Analyzer, dessen Aufbau und Funktionsweise, und zum Endprodukt gibt es in unserem <a href="https://github.com/lukas2311/Audio_Spectrum_Analyser-Lukas-Torben">Projektseiten-Repository.</a>
<p align="center"><img src="https://user-images.githubusercontent.com/42578917/48957578-a9851880-ef59-11e8-9820-1a112041cca9.jpeg" width="400px"></p>
<br>


## Inhaltsverzeichnis
<li><a href="#twooneeight">21.08.18</a></li>
<li><a href="#twoseveneight">27.08.18</a></li>
<li><a href="#twoeighteight">28.08.18</a></li>
<li><a href="#threenine">03.09.18</a></li>
<li><a href="#fournine">04.09.18</a></li>
<li><a href="#tennine">10.09.18</a></li>
<li><a href="#elevennine">11.09.18</a></li>
<li><a href="#sixteennine">16.09.18</a></li>
<li><a href="#seventeennine">17.09.18</a></li>
<li><a href="#eightteennine">18.09.18</a></li>
<li><a href="#fifteenten">15.10.18</a></li>
<li><a href="#eightteenten">18.10.18</a></li>
<li><a href="#twotwoten">22.10.18</a></li>
<li><a href="#twothreeten">23.10.18</a></li>
<li><a href="#twoseventen">27.10.18</a></li>
<li><a href="#twonineten">29.10.18</a></li>
<li><a href="#threeten">30.10.18</a></li>
<li><a href="#sixeleven">06.11.18</a></li>
<li><a href="#twelveeleven">12.11.18</a></li>
<li><a href="#onethreeoneone">13.11.18</a></li>
<li><a href="#onesevenoneone">17.11.18</a></li>
<li><a href="#twooneone">20.11.18</a></li>
<li><a href="#abgabe">23.11.18</a></li>
<br>

## Projekttage
<h3 id="twooneeight">21.08.18 - Unterricht</h3>
An diesem Tag haben wir von Herrn Buhl eine Einführung in das Fach Informatik bekommen und bekamen erklärt, wie wir uns in verschiedene Projekte auf Github einlesen und am besten einen eigenen Entwurf anfertigen können.
<br>
Zudem wurden uns einige Beispielprojekte, wie ein Quadrocopter, ein Arduino Snake-Spiel oder ein Mobile-Game, programmiert mit Greenfoot, gezeigt.

<h3 id="twoseveneight">27.08.18 - Unterricht</h3>
Jetzt begann die Ideenfindung und Recherche zur Umsetzbarkeit des Projektes. Nachdem wir uns auf ein Projekt geeinigt hatten, fingen wir mit der Recherche an: Zunächst benötigten wir einmal ein Verständnis davon, wie digitale Audio-Signale funktionieren und wie diese aufgebaut sind. Zudem haben wir uns ähnliche Projekte angeschaut, um einen weiteren Plan sowie weitere Ideen für unser Projekt zu finden.

<h3 id="twoeighteight">28.08.18 - Unterricht</h3>
Am darauf folgenden Tag haben wir uns mit verschiedenen Hauptplatinen für unser Projekt beschäftigt. Nach Recherche und der Auseinandersetzung mit dem Raspberry Pi, dem Arduino Uno, dem Arduino Mega, dem Texas Instruments MSP430 Launchpad, aber auch unbekannteren Alternativen wie dem Teensy und dem BeagleBone haben wir uns schlussendlich für den Arduino Mega entschieden, einerseits aufgrund der großen Anzahl an Pins und andererseits aufgrund der in der IDE verwendeten Sprache C++, welche für uns eine deutlich stimmigere Synthax aufwies, als z.B. Python. Zudem hat uns auch die große Community hinter Arduino und dem damit verbundenen Support überzeugt. 

<h3 id="threenine">03.09 - Unterricht </h3>
Heute haben wir uns dann mit der näheren Funktionsweise des Arduino Mega beschäftigt. Vor allem vor dem Hintergrund der anschließend verwendeten Bauteile. Dabei haben wir zudem versucht, eine mögliche Umsetzung der Visualisierung aller Frequenzen zu erarbeiten. Wir haben uns dann für LEDs in Verbindung mit Transistoren entschieden.

<h3 id="fournine">04.09 - Unterricht</h3>
An diesem Tag haben wir uns näher mit den verschiedenen Arten von Transistoren und deren unterschiedlichen Dotierungen, sowie den jeweiligen Anwendungsbereichen beschäftigt. Letztendlich haben wir uns für NPN-Transistoren entschieden.

<h3 id="tennine">10.09.18 - Unterricht</h3>
Nun haben wir nähere Planung begonnen. Unser Grundkonzept blieb allerdings unverändert. Wir begannen damit ein Grundkonzept für einen Schaltplan auf draw.io zu zeichnen. 
<br>
<p align="center"><img src="https://user-images.githubusercontent.com/42578917/47315087-d769fb00-d643-11e8-9edb-c32462ccdcd3.png" width="400px"></p>

<h3 id="elevennine">11.09.18 - Unterricht</h3>
Heute haben wir unser Konzept für die Hardware beendet und begonnen, uns mit der endgültigen Programmierumgebung, der Arduino IDE, auseinanderzusetzen und haben uns damit beschäftigt, wie man dort einzelne Pins ansteuert, sowie Inputs an analogen Pins in der IDE ausliest. 

<h3 id="sixteennine">16.09.18 - Zuhause</h3>
Jetzt haben wir recherchiert, was für verschiedene Produkte es gibt, für die Teile die wir brauchen. Auf Amazon und Conrad haben wir dann Teile entdeckt und uns über die Hintergründe der Funktionsweise dieser belesen.

<h3 id="seventeennine">17.09.18 - Unterricht</h3>
Heute haben wir damit begonnen, die endgültigen Teile im Internet rauszusuchen und zu bestellen. Dazu gehörten der Arduino, der MSGEQ7, einige Widerstände, LEDs und Steckbretter mit Jumper-Kabeln. Die Entscheidung dafür beruhte auf der Recherche vom Vortag. Gegen Ende der Stunde haben wir zudem unser weiteres Vorgehen besprochen: wann die Bauteile ankommen, wann wir uns wieder treffen, und wann wir welche Teile fertigstellen.

<h3 id="eightteennine">18.09.18 - Unterricht</h3>
Heute haben wir uns ausgiebiger mit der Verkabelung des MSGEQ7 beschäftigt, wie sie im Datenblatt angegeben ist und unser weiteres Vorgehen besprochen. Zudem haben wir noch weitere benötigte Teile wie 4 weitere Kondensatoren und IC-Fassungen für den MSGEQ7 bestellt. 
Zudem haben wir, nachdem wir die Verkabelung verstanden haben, den Schaltplan beendet: 
<p align="center"><img src="https://user-images.githubusercontent.com/42578917/48625398-67833200-e9af-11e8-848c-5e2630a5e2c4.png" width="400px"></p>

<h3 id="fifteenten">15.10.18 - Zuhause</h3>
Heute haben wir den MSGEQ7 zum ersten Mal mit allen Komponenten angeschlossen und mit dem zuvor geschriebenen Code getestet und 
versucht für verschiedene Songs die Werte über den Seriellen Monitor der Arduino IDE auszulesen. Dadurch war es uns möglich
zuerst vorhandene Fehler zu entdecken und zu beheben.

<h3 id="eightteenten">18.10.18 - Unterricht</h3>
Heute haben wir, Nachdem wir ein bisschen an dem Timing herumgeschraubt haben, mit dem der Analoge Input ausgelesen wird, eine Reihe LEDs mit Transistoren aufgebaut und für die 6. Frequenz angeschlossen, und eine IF-Schleife geschrieben, mit der diese geschaltet werden - als Prototyp. Nach ein paar Korrekturen am Timing funktionierte diese und wir haben einen Durchlauf mit allen 

<h3 id="twotwoten">22.10.18 - Unterricht</h3>
Nun haben wir versucht, mit den gewonnenen Daten etwas anzufangen: Wir haben mehrere If-Schleifen geschrieben, welche dann später
abhängig von den Werten aus dem Seriellen Monitor die einzelnen Transistoren, und damit die einzelnen LEDs schalten. Da der MSGEQ7 nur "Zahlen" als Werte für die stärke der einzelnen Frequenzen ausgibt, können wir an diese Werte auch eine Bedingung knüpfen. Nun haben wir anhand der Werte geschachtelte IF-Schleifen geschrieben, welche jeweils bis zu einem Bestimmten Wert durchlaufen.
<br>
Desweiteren haben wir vor dem Hintergrund des Schaltplans des Arduino Mega eine Pinaufteilung für die verschiedenen LEDs erarbeitet. Dafür haben wir zunächst alle als digitale Ausgänge verfügbare Pins rausgesucht und auf in 7 Reihen unterteilt, für die verschiedenen Frequenzen. Dies haben wir getan, um für LEDs, welche die gleiche Frequenz anzeigen, auch nebeneinanderliegende Pins zu wählen, damit die Schaltung etwas übersichtlicher und nachvollziehbarer wird.

<h3 id="twothreeten">23.10.18 - Unterricht</h3>
An diesem Tag haben wir mit dem endgültigen Code begonnen. Also haben wir zunächst in anbindung an die letzte Stunde eine Menge Variablen geschrieben, in die wir die in der letzten Stunde erarbeitete Pinaufteilung eingetragen haben. So hat jeder Transistor, also jede LED einen Pin auf dem Arduino bekommen. Um diese Wiederzuerkennen, haben wir ein Benennungssystem entwickelt. Zudem haben wir die IF-Schleifen um die jeweiligen zugehörigen Pins ergänzt und die jeweiligen Schaltungen hinzugefügt.

<h3 id="twoseventen">27.10.18 - Zuhause</h3>
Nun haben wir mit der Aufteilung der LEDs und Transistoren befasst und damit begonnen diese auf die Platinen zu löten. Dabei haben wir sowohl Widerstände, Transistoren, LEDs und Kabel festgelötet und erste Tests an der fertigen Platine durchgeführt um zu prüfen, ob alle LEDs und Transistoren ordnungsgemäß funktionieren und zu schauen, ob auch alle Transistoren und LEDs richtig gepolt verlötet wurden.

Nach einigen Korrekturen und zwei neu-eingelöteten LEDs haben die LEDs alle funktioniert und wir konnten mit der Verkabelung weitermachen. Dafür haben wir zwei "Aufsteck-Platinen" für den Arduino gelötet, an die wir dann die Kabel anlöten, damit wir auch nachträglich noch änderungen machen können und wir den Arduino nicht mit der Hitze beschädigen. Nach Fertigstellung könnte so der Arduino einfach aufgesteckt werden.

<h3 id="twonineten">29.10.18 - Unterricht</h3>
Heute haben wir unsere Projektseite weitergeführt. Zum einen den Hardware-, aber vorallem auch den Softwareteil haben wir dabei weiter fortgeführt. Außerdem haben wir Ergänzungen am Stundenprotokoll vorgenommen.

<h3 id="threeten">30.10.18 - Unterricht</h3>
Nun haben wir uns um den Aufbau und das Aussehen unserer Dokumentation gekümmert. Dazu haben wir Überschriften formatiert, Bilder eingebunden und recherchiert wie wir ein Inhaltsverzeichnis erstellen können, welches auf daie jeweilige Überschrift verweist. Außerdem haben wir herausgefunden, wie es möglich ist, Videos in GitHub-Repositories einzubauen.

<h3 id="sixeleven">06.11.18 - Unterricht</h3>
Wir haben nun weiter und zielgerichteter an unserer Dokumentation gearbeitet. Dabei haben wir ein Inhaltsverzeichnis und eine Komponentenliste mit jeweiliger Verlinkung erstellt und weiter am Menüpunkt Hardware gearbeitet und einen Text zum MSGEQ7 geschrieben und wie dieser funktioniert, verbunden mit dem zugehörigen Strobe-Diagramm. 

<h3 id="twelveeleven">12.11.18 - Unterricht</h3>
Heute haben wir uns mit der Konzeption eines Gehäuses für den Audio Spectrum Analyser beschäftigt. Dabei haben wir geplant, wo welche Ausgänge, Knöpfe usw. hinkommen, und wie die konkreten Außenmaße, sowie der Platzbedarf für die Komponenten innerhalb des Gehäuses sein sollen.

<h3 id="onethreeoneone">13.11.18 - Unterricht</h3>
Diesmal haben wir weiter an unserer Dokumentation gearbeitet. Wir haben den Bereich Software erweitert um den Code für den Reset am MSGEQ7 und die jeweiligen Grafiken Codeschnipsel eingefügt. 

<h3 id="onesevenoneone">17.11.18 - Zuhause</h3>
Heute haben wir die benötigten Widerstände auf der Platine festgelötet und alles verkabelt. Danach haben wir alle Bauteile im Gehäuse befestigt. Außerdem haben wir die Dokumentation weiter bearbeitet.

<h3 id="twooneone">20.11.18 - Unterricht</h3>
Dies war der letzte Tag, an dem wir im Unterricht an unseren Projekten arbeiten konnten. Da wir unser Projekt so gut wie fertig hatten, haben wir uns vor allem mit dem Testen und mit minimalen Veränderungen am Timing der LEDs zur Musik beschäftigt. Das Timing, was in den IF-Schleifen entscheidet, bei welchem vom MSGEQ7 zurückgegebenen Wert, eine jeweilige LED angeschaltet wird.

<h3 id="abgabe">23.11 - Abgabe</h3>
Heute haben wir Fotos und Videos vom fertigen Produkt gemacht und diese in unsere Repositories eingebunden. Außerdem haben wir letzte Ergänzungen und Korrekturen an der Projektseite und dem Stundenprotokoll vorgenommen.
