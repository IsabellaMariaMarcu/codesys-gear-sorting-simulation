\# Förderbandsimulation mit Zahnraderkennung | CODESYS



Simulation eines SPS-gesteuerten Förderbands, das Zahnräder mit kleinen und großen Bohrungen mithilfe eines Prüfzylinders und simulierter Sensoren unterscheidet.



\## Demo



\[Video der Visualisierung ansehen](demo.mp4)



\## Funktionsweise



1\. Das Förderband transportiert ein Zahnrad zum Positionssensor.

2\. Das Förderband stoppt und der Prüfzylinder fährt aus.

3\. Bei einer großen Bohrung erreicht der Zylinder seine vordere Endlage.

4\. Bei einer kleinen Bohrung wird der Zylinder blockiert. Nach einer Sekunde ohne Endlagensignal wird das Zahnrad als Zahnrad mit kleiner Bohrung erkannt.

5\. Die entsprechende Kontrolllampe leuchtet und der zugehörige Zähler wird erhöht.

6\. Der Zylinder wird eingefahren. Nach einer Wartezeit von 0,5 Sekunden startet das Förderband erneut.



\## Umsetzung



\- Programmierung in Structured Text nach IEC 61131-3

\- Schrittweise Ablaufsteuerung

\- Zeitüberwachung mit TON-Timern

\- Getrennte Zähler für beide Zahnradtypen

\- CODESYS-Visualisierung mit Bedientasten und Statusanzeigen

\- Separates Simulationsprogramm für Förderbandbewegung, Zylinderbewegung und Sensorsignale



\## Software



Entwickelt mit CODESYS V3.5 SP22 Patch 3.



\## Simulation starten



1\. Dieses Repository herunterladen oder klonen.

2\. Die Datei `SmallHoleGear\_BigHoleGear\_ConveyerBelt.project` in CODESYS öffnen.

3\. Den Simulationsmodus aktivieren, einloggen und die Anwendung starten.

4\. Die Visualisierung `Visu\_Main` öffnen.

5\. Über die Schaltflächen Zahnräder mit großer oder kleiner Bohrung einfügen und den Ablauf beobachten.

