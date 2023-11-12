# Personenwaage-mit-externer-drahtloser-Anzeige
# 1-Einleitung

In diesem Projektbericht wird die Entwicklung einer innovativen Personenwaage mit
externer Anzeige über Wi-Fi unter Verwendung des Mikrocontrollers ESP32 beschrieben.
Die heutige Technologie ermöglicht uns, Alltagsgegenstände mit intelligenten Funktionen
auszustatten, um unser Leben komfortabler und effizienter zu gestalten. Die
Personenwaage ist ein solches Gerät, das in nahezu jedem Haushalt zu finden ist. Indem wir
sie mit Wi-Fi-Fähigkeiten und einem leistungsstarken Mikrocontroller erweitern, können wir
die Funktionalität der Waage erheblich verbessern.

Unser Ziel bei diesem Projekt war es, eine Personenwaage zu entwickeln, die über Wi-Fi
eine externe Anzeige ermöglicht. Dadurch soll es dem Benutzer ermöglicht werden, seine
Gewichtsdaten drahtlos an ein Smartphone, Tablet oder einen Computer zu übertragen und
sie dort bequem zu verfolgen und auszuwerten. Dieser Ansatz ermöglicht eine nahtlose
Integration der Personenwaage in das moderne vernetzte Zuhause und bietet dem Benutzer
zahlreiche Vorteile.

Der ESP32 ermöglicht die drahtlose Kommunikation mit anderen Geräten über das Internet,
was ideal für die Übertragung von Gewichtsdaten von der Waage zur externen Anzeige ist.
Im Verlauf dieses Berichts werden wir detailliert auf die verschiedenen Phasen des Projekts
eingehen, von der Konzeption und dem Design bis hin zur Implementierung und Validierung
der entwickelten Personenwaage mit externer Anzeige. Wir werden auch auf
Herausforderungen, Lösungsansätze und die erzielten Ergebnisse eingehen.
Dieses Projekt stellt einen bedeutenden Fortschritt in Bezug auf die Funktionalität und
Konnektivität von Personenwaagen dar und bietet dem Benutzer eine bequeme und einfach
zu bedienende Methode zur Überwachung seines Gewichts.

# 2-PROJEKTZIELE

Die Hauptziele des Projekts waren: 
-	Integration einer Personenwaage mit einem ESP32-Mikrocontroller zur Gewichtsmessung. 
-	Einrichtung einer WLAN-Kommunikation zwischen dem ESP32 und einem PC. 
-	Übertragung der Gewichtsdaten drahtlos an den PC. 
-	Anzeige und Verarbeitung der Gewichtsdaten auf dem PC. 
-	Erstellen für jede Person ein Profil und speichern die Daten

# 3-HARDWARE-KOMPONENTEN

Für dieses Projekt wurden folgende Hardware-Komponenten verwendet: 

# 3.1	Personenwaage

Dieser Sensor der Personenwaage besteht aus Wägezellen, die das Gewicht der Person erfassen und in elektrische Signale umwandeln. Diese Signale werden dann mithilfe des ESP32-Mikrocontrollers verarbeitet. 
Zusätzlich haben wir in der Personenwaage eine Brückenschaltung mit 8 Widerständen implementiert. 
Diese Widerstände sind als diagonale Halbbrücke angeordnet, um eine präzise und genaue 
Gewichtsmessung zu ermöglichen. Die Brückenschaltung erfasst die winzigen Veränderungen in den Widerstandswerten der Wägezellen und wandelt sie in ein Ausgangssignal um, das proportional zum Gewicht der Person ist. 
Durch die Verwendung dieser Brückenschaltung können wir die Empfindlichkeit und Genauigkeit der Gewichtsmessung verbessern. Der ESP32-Mikrocontroller nimmt dieses Ausgangssignal auf und führt die entsprechenden Berechnungen durch, um das Gewicht der Person anzuzeigen und gegebenenfalls weitere Funktionen der Personenwaage zu steuern. 
Mit dieser sorgfältig gestalteten Integration des Personengewichtssensors und der Brückenschaltung können wir präzise und zuverlässige Gewichtsmessungen für unsere Personenwaage gewährleisten. 
              ![image](https://github.com/KavianBahrehdar/Personenwaage-mit-externer-drahtloser-Anzeige/assets/115076717/91a30ca2-bb0e-4af6-bd9c-b3f1c952513b)

# 3.2	Der ESP32-Mikrocontroller 

Der ESP32-Mikrocontroller spielt eine zentrale Rolle in diesem Projekt. Er übernimmt die Aufgabe der 
Datenerfassung, -verarbeitung und -übertragung. Der Mikrocontroller ist mit dem 
Personengewichtssensor verbunden und empfängt die elektrischen Signale, die das Gewicht der Person repräsentieren. Mithilfe seiner leistungsstarken Rechenleistung kann der ESP32 das Gewicht präzise und schnell berechnen. 

# 3.3	Externe Anzeige (PC) 

Für die externe Anzeige wurde ein PC ausgewählt, um die Gewichtsmessungen der Personenwaage darzustellen. Die Entscheidung für einen PC als Anzeigegerät bietet den Vorteil eines größeren 
Bildschirms und einer vielfältigen Darstellungsmöglichkeit der Messergebnisse. Dies ermöglicht eine klare und benutzerfreundliche Anzeige der Gewichtsdaten. 
Um die Kommunikation zwischen der Personenwaage und dem PC zu ermöglichen, wurde eine spezielle Anwendungssoftware entwickelt. Die Software wurde in der Programmiersprache Python geschrieben und bietet eine benutzerfreundliche Schnittstelle zur Anzeige der Gewichtsmessungen. Die Verwendung von Python ermöglichte eine einfache und effiziente Implementierung der Softwarefunktionen. 
Die App auf dem PC ermöglicht es dem Benutzer, die Gewichtsmessungen in Echtzeit zu empfangen und anzuzeigen. Die Messergebnisse werden übersichtlich auf dem Bildschirm präsentiert und können je nach den Anforderungen des Benutzers angepasst werden. Darüber hinaus bietet die App zusätzliche Funktionen wie das Speichern der Messdaten, die Einrichtung von Benutzerprofilen und die Verfolgung des Gewichtsverlaufs im Laufe der Zeit. 

# 3.4	Die Platine 

![image](https://github.com/KavianBahrehdar/Personenwaage-mit-externer-drahtloser-Anzeige/assets/115076717/f6f0a01b-c4fb-4e56-aa44-9e5f5f4530c6)








