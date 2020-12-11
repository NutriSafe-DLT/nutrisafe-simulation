# Simulationsmodell: IT-Vorfall oder Pandemie (Szenario Bio-Kochschinken)
Das Modell erlaubt die Simulation der Krisenszenarien IT-Vorfall (in Form einer sich ausbreitenden Schadsoftware) und Pandemie. Das modell wurde von Jens Blume mit Unterstützung durch Manfred Hofmeier am Institut für Schutz und Zuverlässigkeit der Universität der Bundeswehr München entwickelt.

## Anwendung
![Screenshot](../screenshots/mdl_screenshot_bioschinken_it-vorfall_pandemie.png)
Mit dem Modell können die folgenden Krisenszenarien simuliert werden. Dabei wird die Resilienz primär über die Bedarfsdeckung beim Endverbraucher bemessen.

### Simulation des Krisenszenarios IT-Vorfall
Die Krise IT-Vorfall wird mit dem Button "IT-Krise starten" ausgelöst. Dabei können zuvor folgende Parameter angepasst werden:

* Startpunkt: Ein zufälliger Akteur in der angegebenen Gruppe ist der erste von der Schadsoftware infizierte Akteur im Wertschöpfungsnetzwerk
* Produktionseinbußen: Einbußen in der Produktion durch die Schadsoftware (Faktor in Prozent)
* Ausbreitungswahrscheinlichkeit: Jedesmal wenn ein infizierter Akteur Kontakt mit einem anderen Akteur hat, kann er mit der angegebenen Wahrscheinlichkeit den Kontaktpartner infizieren
* Infektionsdauer: Dauer, bis die Infektion (Schadsoftware) bereinigt ist. Für die Dauer der Infektion gelten die Produktionseinbußen und der Akteur kann andere Akteure mit der angegebenen Wahrscheinlichkeit infizieren.

### Simulation des Krisenszenarios Pandemie
Die Krise Pandemie wird mit dem Button "Pandemie starten" ausgelöst. Dabei können zuvor folgende Parameter angepasst werden:

* Population in Quarantäne: Agentenpopulation, die von Quarantänemaßnahmen betroffen ist
* Anteil betroffener Agenten
* Produktionseinbußen durch Quarantäne
* Dauer der Quarantäne
* Globale Produktionseinbußen: Einbußen der Produktion (in Prozent) über alle Akteure im gesamten Wertschöpfungsnetzwerk.

### Simulation des potentiellen Einflusses von DLT
Um den möglichen Einfluss der Nutzung von Distributed-Ledger-Technologie (DLT) auf den Verlauf von Krisenszenarien zu untersuchen, können die Simulationsmodelle wie folgt angewandt werden:

#### DLT im Krisenszenario IT-Vorfall:
Der Einfluss von DLT auf das Krisenszenario IT-Vorfall kann durch Variation der folgenden Parameter untersucht werden:

* Produktionseinbußen: Da in einer DLT die Daten weniger anfällig für illegitime Veränderungen etwa durch Schadsoftware sind (Integrität) und die wichtigsten Daten (z.B. zur Chargendokumentation) weinterhin verfügbar sind, kann ein geringer Faktor für die Produktionseinbußen angenommen werden.
* Ausbreitungswahrscheinlichkeit: Wird mehr Interaktion entlang der Wertschöpfungskette (z.B. Übermittlung von Daten) mittels DLT abgewickelt, wird weniger über klassische Kanäle wie etwa Email kommuniziert, welche eine Schadsoftware übertragen können. Daher kann eine geringere Ausbreitungswahrscheinlichkeit angenommen werden.

#### DLT im Krisenszenario Pandemie:
Der Einfluss von DLT auf das Krisenszenario Pandemie kann durch Variation der folgenden Parameter untersucht werden:

* Anteil betroffener Agenten: Findet mehr digitale Kommunikation und Dokumentenübergabe statt, reduziert das physische Kontakte zwischen den Akteuren. Damit kann ein geringerer Anteil an betroffenen Akteuren angenommen werden.

## Analyse
Die Resilienz wird in diesem Modell über die Bedarfsdeckung beim Endverbraucher bemessen. Es sollten hierfür mehrere Iterationen der Simulation je Parametereinstellung durchgeführt werden, da einige Abläufe von zufälligen Werten abhängen.

## Lizenz
![CC-BY](https://i.creativecommons.org/l/by/4.0/88x31.png)

Dieses Werk ist lizenziert unter einer [Creative Commons Namensnennung 4.0 International Lizenz](http://creativecommons.org/licenses/by/4.0/).

## Danksagung
Wir danken dem Bundesministerium für Bildung und Forschung (BMBF) für die Möglichkeit der Forschung im Rahmen des Projektes NutriSafe (FKZ 13N15070 bis 13N15076) sowie dem Sicherheitsforschungsförderprogramm KIRAS, finanziert vom Bundesministerium für Landwirtschaft, Regionen und Tourismus (Projektnummer: 867015).


