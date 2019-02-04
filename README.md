# TTGO v2.1 Workshop

In diesem Repository haben wir einen einfachen Workshop mit einem TTGO LoRa32 v2.1 erstellt.

Der Workshop ist kein Low-Power Workshop, d.h. die Stromsparfunktionen des TTGO LoRa32 werden nicht ausgenutzt (kein Deep Sleep) und das OLED Display wird dauerhaft die gemessenen Daten anzeigen. Auch der Quellcode ist einfach gehalten, um einen unerfahrenen Anwender nicht mit bspw. "includes" und Klassen zu überfordern.

Wir freuen uns selbstverständlich über weitere Anregungen oder Pull-Request, um die Lektionen zu erweitern. Solltet ihr diesen Workshop auch bei euch durchführen, würden wir uns über eine kurze Nachricht freuen.

# Hardwarevorraussetzungen

  * TTGO LoRa32 v2.1 (andere Versionen sollten auch funktioieren, aber der Workshop wird mit diesem Modell durchgeführt)
  * Bosch BME280 Modul (Temperatur, Luftdruck, Luftfeuchtigkeit)

# Entwicklungsumgebung / Installation

Die Arduino IDE kann unter http://www.arduino.cc heruntergeladen werden. Der Download befindet sich auf der Webseite unter **"Software**, **Downloads"**. Hier sollte der Windows Installer verwendet und gestartet werden. 
Nach der Installation muss noch die Unterstützung für den auf dem TTGO Board eingesetzten Mikrocontroller, den Espressif ESP32, eingebunden werden. Dazu wird die Arduino IDE gestartet und folgende Schritte durchgeführt:

  1. Öffnen von **"Datei**, **Voreinstellungen"**
  2. Unter **"Zusätzliche Boardverwalter-URLs"** folgende Adresse hinzufügen: **https://dl.espressif.com/dl/package_esp32_index.json**
  3. Unter **"Werkzeuge**, **Board**, **Boardverwalter"** den Suchbegriff **"ESP32"** eingeben.
  4. Mit **"Installieren"** die Installation des Boards in der Arduino IDE starten.
  5. Unter **"Werkzeuge**, **Board"** das Board **"TTGO LoRa32-OLED V1"** auswählen.

Die Entwicklungsumgebung ist jetzt für das Entwicklungsboard eingerichtet und die einzelnen Beispiele können nun durchgeführt werden.

# Lektionen

Nachfolgend werden die einzelnen Lektionen des Workshops durchgeführt. Alle Verzeichnisse enthalten einen fertigen Beispielsketch, in dem die Aufgabe der Lektionen bereits durchgeführt wurden.

  1. [Lektion 1 - Sensor auslesen](./Lektion 1/README.md)
  2. Lektion 2 - Sensorwerte auf dem Display ausgeben
  3. Lektion 3 - Sensorwerte mit LoRaWAN und dem The Things Network übertragen