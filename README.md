# Stunden-Tagebuch -- Informatik-Projekt-Torben-Lukas 

### 21.08.18 - Unterricht
An diesem Tag bekamen wir von Herrn Buhl eine Einführung in das Fach Informatik bekommen und bekamen erklärt, wie wir uns in verschiedene Projekte auf Github einlesen und am besten einen eigenen Entwurf anfertigen können.
<br><br>
Zudem wurden uns einige Beispielprojekte, wie ein Quadrocopter, ein Arduino Snake-Spiel oder ein Mobile-Game, programmiert mit Greenfoot, gezeigt.

### 27.08.18 - Unterricht
Jetzt begann die Ideenfindung und Recherche zur Umsetzbarkeit des Projektes. Nachdem wir uns auf ein Projekt geeinigt hatten, fingen wir mit der Recherche an: Zunächst benötigten wir einmal ein Verständnis davon, wie digitale Audio-Signale funktionieren und wie diese aufgebaut sind. Zudem haben wir uns ähnliche Projekte angeschaut, um einen weiteren Plan sowie weitere Ideen für unser Projekt zu finden.
<br><br>
Ausserdem haben wir uns mit verschiedenen Hauptplatinen für unser Projekt beschäftigt. Nach Recherche und der Auseinandersetzung mit dem Raspberry Pi, dem Arduino Uno, dem Arduino Mega, dem Texas Instruments MSP430 Launchpad, aber auch unbekannteren Alternativen wie dem Teensy und dem BeagleBone haben wir uns schlussendlich für den Arduino Mega entschieden, einerseits aufgrund der großen Anzahl an Pins, und andererseits aufgrund der in der IDE verwendeten Sprache C++, welche für uns eine deutlich stimmigere Synthax aufwies, als z.B. Python. Zudem hat uns auch die große Community hinter Arduino und dem damit verbundenen Support überzeugt. 

### 28.08.18 - Unterricht
Heute haben wir uns dann mit der näheren Funktionsweise des Arduino Mega beschäftigt. Vor allem vor dem Hintergrund der anschließend verwendeten Bauteile. Dabei haben wir zudem versucht, eine mögliche Umsetzung der Visualisierung aller Frequenzen zu erarbeiten. Wir haben uns dann für LEDs in Verbindung mit Transistoren entschieden, was uns dazu brachte, uns näher mit den verschiedenen Arten von Transistoren, wie dem NPN, dem PNP und dem Mosfet und deren unterschiedlichen Dotierungen sowie den jeweiligen Anwendungsbereichen zu beschäftigen.

### 03.09

### 04.09

### 10.09.18 - Unterricht
Nun haben wir nähere Planung begonnen. Unser Grundkonzept blieb allerdings unverändert. Wir begannen damit ein Grundkonzept für einen Schaltplan auf draw.io zu zeichnen. 
<br>
<p align="center"><img src="https://user-images.githubusercontent.com/42578917/47315087-d769fb00-d643-11e8-9edb-c32462ccdcd3.png" width="400px"></p>

### 11.09.18 - Unterricht
Heute haben wir unser Konzept für die Hardware beendet und begonnen, uns mit der endgültigen Programmierumgebung, der Arduino IDE auseinanderzusetzen und haben uns damit beschäftigt, wie man dort einzelne Pins ansteuert, sowie Inputs an analogen Pins in der IDE ausliest. 

### 16.09.18 - Zuhause
Jetzt haben wir recherchiert, was für verschiedene Produkte es gibt, für die Teile die wir brauchen. Auf Amazon und Conrad haben wir dann Teile entdeckt und uns über die Hintergründe der Funktionsweise dieser belesen.

### 17.09.18 - Unterricht
Heute haben wir damit begonnen, die endgültigen Teile im Internet rauszusuchen und zu bestellen. Dazu gehörten der Arduino, der MSGEQ7 einige Widerstände, LEDs und Steckbretter mit Jumper-Kabeln. Die Entscheidung dafür beruhte auf der Recherche vom Vortag. Gegen Ende der Stunde haben wir zudem unser weiteres Vorgehen besprochen: wann die Bauteile ankommen, wann wir uns wieder treffen, und wann wir welche Teile fertigstellen.

### 18.09.18 - Unterricht
Heute haben wir uns ausgiebiger mit der Verkabelung des MSGEQ7 beschäftigt, wie sie im Datenblatt angegeben ist und unser Weiteres vorgehen besprochen. Zudem haben wir noch weitere benötigte Teile wie 4 weitere Kondensatoren und IC-Fassungen für den MSGEQ7 bestellt. 

Zudem haben wir, nachdem wir die Verkabelung verstanden haben, den Schaltplan beendet: 

<p align="center"><img src="https://user-images.githubusercontent.com/42578917/48625398-67833200-e9af-11e8-848c-5e2630a5e2c4.png" width="400px"></p>

### 15.10.18 - Zuhause
Heute haben wir den MSGEQ7 zum ersten mal mit allen Komponenten angeschlossen und mit dem zuvor geschreibenen Code getestetet und 
versucht für verschiedene Songs die Werte über den Seriellen Monitor der Arduino IDE auszulesen. Dadurch war es uns möglich,
zuerst vorhandene Fehler zu entdecken und zu beheben.

Nachdem wir ein bisschen an dem Timing herumgeschraubt haben, mit dem der Analoge Input ausgelesen wird, haben wir eine Reihe LEDs mit Transistoren aufgebaut und für die 6. Frequenz angeschlossen, und eine IF-Schleife geschrieben, mit der diese geschaltet werden - als Prototyp. Nach ein paar Korrekturen am Timing funktionierte diese und wir haben einen Durchlauf mit allen 
### 18.10.18 - Unterricht
### 22.10.18 - Unterricht
Nun haben wir versucht, mit den gewonnenen Daten etwas anzufangen: Wir haben mehrere If-Schleifen geschrieben, welche dann später
abhängig von den Werten aus dem Seriellen Monitor die einzelnen Transistoren, und damit die einzelnen LEDs schalten. Da der MSGEQ7 nur "Zahlen" als Werte für die stärke der einzelnen Frequenzen ausgibt, können wir an diese Werte auch eine Bedingung knüpfen. Nun haben wir anhand der Werte geschachtelte IF-Schleifen geschrieben, welche jeweils bis zu einem Bestimmten Wert durchlaufen.
<br><br>
Desweiteren haben wir vor dem Hintergrund des Schaltplans des Arduino Mega eine Pinaufteilung für die verschiedenen LEDs erarbeitet. Dafür haben wir zunächst alle als digitale Ausgänge verfügbare Pins rausgesucht und auf in 7 Reihen unterteilt, für die verschiedenen Frequenzen. Dies haben wir getan, um für LEDs, welche die gleiche Frequenz anzeigen, auch nebeneinanderliegende Pins zu wählen, damit die Schaltung etwas übersichtlicher und nachvollziehbarer wird.

### 23.10.18 - Unterricht
An diesem Tag haben wir mit dem endgültigen Code begonnen. Also haben wir zunächst in anbindung an die letzte Stunde eine Menge Variablen geschrieben, in die wir die in der letzten Stunde erarbeitete Pinaufteilung eingetragen haben. So hat jeder Transistor, also jede LED einen Pin auf dem Arduino bekommen. Um diese Wiederzuerkennen, haben wir ein Benennungssystem entwickelt. Zudem haben wir die IF-Schleifen um die jeweiligen zugehörigen Pins ergänzt und die jeweiligen Schaltungen hinzugefügt.

Außerdem haben wir unsere Dokumentation weitergeführt. Sowohl den Hardware-, als auch den Softwareteil haben wir dabei weiter fortgeführt.

### 27.10.18 - Zuhause
Nun haben wir mit der Aufteilung der LEDs und Transistoren befasst und damit begonnen diese auf die Platinen zu löten. Dabei haben wir sowohl Widerstände, Transistoren, LEDs und Kabel festgelötet und erste Tests an der fertigen Platine durchgeführt um zu prüfen, ob alle LEDs und Transistoren ordnungsgemäß funktionieren und zu schauen, ob auch alle Transistoren und LEDs richtig gepolt verlötet wurden.

Nach einigen Korrekturen und zwei neu-eingelöteten LEDs haben die LEDs alle funktioniert und wir konnten mit der Verkabelung weitermachen. Dafür haben wir zwei "Aufsteck-Platinen" für den Arduino gelötet, an die wir dann die Kabel anlöten, damit wir auch nachträglich noch änderungen machen können und wir den Arduino nicht mit der Hitze beschädigen. Nach Fertigstellung könnte so der Arduino einfach aufgesteckt werden.

### 29.10.18 - Unterricht
### 28.10.18 - Unterricht
### 06.11.18 - Unterricht
Wir haben nun weiter und zielgerichteter an unserer Dokumentation gearbeitet. Dabei haben wir ein Inhaltsverzeichnis und eine Komponentenliste mit jeweiliger Verlinkung erstellt und weiter am Menüpunkt Hardware gearbeitet und einen Text zum MSGEQ7 geschrieben und wie dieser funktioniert, verbunden mit dem zugehörigen Strobe-Diagramm. 

### 12.11.18 - Unterricht
Heute haben wir uns mit der Konzeption eines Gehäuses für den Audio Spectrum Analyser beschäftigt. Dabei haben wir geplant, wo welche Ausgänge, Knöpfe usw. hinkommen, und wie die konkreten Außenmaße, sowie der Platzbedarf für die Komponenten innerhalb des Gehäuses sein sollen.

### 13.11.18 - Unterricht
Diesmal haben wir weiter an unserer Dokumentation gearbeitet. Wir haben den Bereich Software erweitert um den Code für den Reset am MSGEQ7 und die jeweiligen Grafiken Codeschnipsel eingefügt. 

### 17.11.18 - Zuhause
Heute haben wir die benötigten Widerstände auf der Platine festgelötet und alles verkabelt. Danach haben wir alle Bauteile im Gehäuse befestigt. Außerdem haben wir die Dokumentation weiter bearbeitet.
