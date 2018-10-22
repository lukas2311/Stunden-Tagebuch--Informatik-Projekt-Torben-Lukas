# Stunden-Tagebuch -- Informatik-Projekt-Torben-Lukas 

### 21.08.18 - Unterricht
An diesem Tag bekamen wir von Herrn Buhl eine Einführung in das Fach Informatik bekommen und bekamen erklärt, wie wir uns in verschiedene Projekte auf Github einlesen und am besten einen eigenen Entwurf anfertigen können.
<br><br>
Zudem wurden uns einige Beispielprojekte, wie ein Quadrocopter, ein Arduino Snake-Spie oder ein Mobile-Game, programmiert mit Greenfoot, gezeigt.
### 27.08.18 - Unterricht
Jetzt begann die Ideenfindung und Recherche zur Umsetzbarkeit des Projektes. Nachdem wir uns auf ein Projekt geeinigt hatten, fingen wir mit der Recherche an: Zunächst benötigten wir einmal ein Verständnis davon, wie digitale Audio-Signale funktionieren und wie diese aufgebaut sind. Zudem haben wir uns ähnliche Projekte angeschaut, um einen weiteren Plan sowie weitere Ideen für unser Projekt zu finden.
<br><br>
Ausserdem haben wir uns mit verschiedenen Hauptplatinen für unser Projekt beschäftigt. Nach Recherche und der Auseinandersetzung mit dem Raspberry Pi, dem Arduino Uno, dem Arduino Mega, dem Texas Instruments MSP430 Launchpad, aber auch unbekannteren Alternativen wie dem Teensy und dem BeagleBone haben wir uns schlussendlich für den Arduino Mega entschieden, einerseits aufgrund der großen Anzahl an Pins, und andererseits aufgrund der in der IDE verwendeten Sprache C++, welche für uns eine deutlich stimmigere Synthax aufwies, als z.B. Python. Zudem hat uns auch die große Community hinter Arduino und dem damit verbundenen Support überzeugt. 
### 28.08.18 - Unterricht
Heute haben wir uns dann mit der näheren Funktionsweise des Arduino Mega beschäftigt. Vor allem vor dem Hintergrund der anschließend verwendeten Bauteile. Dabei haben wir zudem versucht, eine mögliche Umsetzung der Visualisierung aller Frequenzen zu erarbeiten. Wir haben uns dann für LEDs in Verbindung mit Transistoren entschieden, was uns dazu brachte, uns näher mit den verschiedenen Arten von Transistoren, wie dem NPN, dem PNP und dem Mosfet und deren unterschiedlichen Dotierungen sowie den jeweiligen Anwendungsbereichen zu beschäftigen.
### 10.09.18 - Unterricht
Nun haben wir nähere Planung begonnen. Unser Grundkonzept blieb allerdings unverändert. Wir begannen damit ein Grundkonzept für einen Schaltplan auf draw.io zu zeichnen. 
<br>
<p align="center"><img src="https://user-images.githubusercontent.com/42578917/47315087-d769fb00-d643-11e8-9edb-c32462ccdcd3.png" width="400px"></p>

### 11.09.18 - Unterricht
Heute haben wir unser Konzept für die Hardware beendet und begonnen, uns mit der endgültigen Programmierumgebung, der Arduino IDE auseinanderzusetzen und haben uns damit beschäftigt, wie man dort einzelne Pins ansteuert, sowie Inputs an analogen Pins in der IDE ausliest 
### 17.09.18 - Unterricht
Heute haben wir damit begonnen, die endgültigen Teile im Internet rauszusuchen und zu bestellen. Dazu gehörten der Arduino, der MSGEQ7 einige Widerstände, LEDs und Steckbretter mit Jumper-Kabeln 
### 18.09.18 - Unterricht
Heute haben wir uns ausgiebiger mit der Verkabelung des MSGEQ7 beschäftigt, wie sie im Datenblatt angegeben ist und unser Weiteres vorgehen besprochen. Zudem haben wir noch weitere benötigte Teile wie 4 weitere Kondensatoren und IC-Fassungen für den MSGEQ7 bestellt.  
### 15.10.18 - Zuhause
Heute haben wir den MSGEQ7 zum ersten mal mit allen Komponenten angeschlossen und mit dem zuvor geschreibenen Code getestetet und 
versucht für verschiedene Songs die Werte über den Seriellen Monitor der Arduino IDE auszulesen. Dadurch war es uns möglich,
zuerst vorhandene Fehler zu entdecken und zu beheben. 
### 22.10.18 - Unterricht
Nun haben wir versucht, mit den gewonnenen Daten etwas anzufangen: Wir haben mehrere If-Schleifen geschrieben, welche dann später
abhängig von den Werten aus dem Seriellen Monitor die einzelnen Transistoren, und damit die einzelnen LEDs schalten. Da der MSGEQ7 nur "Zahlen" als Werte für die stärke der einzelnen Frequenzen ausgibt, können wir an diese Werte auch eine Bedingung knüpfen. Nun haben wir anhand der Werte geschachtelte IF-Schleifen geschrieben, welche jeweils bis zu einem Bestimmten Wert durchlaufen.
<br>
Desweiteren haben wir vor dem Hintergrund des Schaltplans des Arduino Mega eine Pinaufteilung für die verschiedenen LEDs erarbeitet. Dafür haben wir zunächst alle als digitale Ausgänge verfügbare Pins rausgesucht und auf in 7 Reihen unterteilt, für die verschiedenen Frequenzen. Dies haben wir getan, um für LEDs, welche die gleiche Frequenz anzeigen, auch nebeneinanderliegende Pins zu wählen, damit die Schaltung etwas übersichtlicher und nachvollziehbarer wird.
### 23.10.18 - Unterricht
An diesem Tag haben wir mit dem endgültigen Code begonnen. Also haben wir zunächst in anbindung an die letzte Stunde eine Menge Variablen geschrieben, in die wir die in der letzten Stunde erarbeitete Pinaufteilung eingetragen haben. So hat jeder Transistor, also jede LED einen Pin auf dem Arduino bekommen. Um diese Wiederzuerkennen, haben wir ein Benennungssystem entwickelt. Zudem haben wir die IF-Schleifen um die jeweiligen zugehörigen Pins ergänzt und die jeweiligen Schaltungen hinzugefügt.
