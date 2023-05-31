# Grundwasser-digital

## Inhaltsverzeichnis
* [Kurzbeschreibung](#Kurzbeschreibung)
* [Installation](#Installation)
* [Verwendung](#Verwendung)
* [Lizenz](#Lizenz)
* [Credits](#Credits)
* [Förderhinweis](#Förderhinweis)



Kurzbeschreibung: Dieses Projekt besteht aus zwei interaktiven digitalen Exponaten, die in der Ausstellung "Grundwasser lebt!" eingesetzt werden:

### 1. Volumetrisches Display (Voxon VX1, Leap Motion Handerkennung)
**Unity-Projekt: GRUNDWASSER_digital_VOXON_VX1**

Mit diesem Exponat können Grundwassertiere näher inspiziert werden. Das Exponat stellt die Lebewesen in einem volumetrischen Display dar und erlaubt es die Tiere über eine Handerkennung von allen Seiten zu betrachten und auch zu vergrößern.

### 2. Immersive Wall (3 x 4k-Display (86"), zwei Joysticks zur Steuerung)
**Unity-Projekt: GRUNDWASSER_digital_BIGSCREEN**

Dieses Exponat erlaubt eine Tauchfahrt in einen Grundwasserleiter. Die Steuerung erfolgt über zwei Joysticks, die an einer Konsole vor drei großen hochauflösenden Displays angebracht ist. Die Gesamtauflösung des Bildschirmes beträgt 6480 x 3840 Pixel. Beide Anwendungen sind über ein Netzwerk miteinander verbunden, können aber auch separat verwendet werden.

Der Aufbau und die Funktion der Anwendungen sind in diesem Video zu sehen:
https://vimeo.com/745168832

## Voraussetzungen:

### Volumetrisches Display (Unity-Projekt: GRUNDWASSER_digital_VOXON_VX1)

- Voxon VX1 (kann auch simuliert werden, siehe Voxon SDK)
https://voxon.co/voxon-vx1-available-for-purchase/
- Leap Motion Sensor (ist für die Interaktionen mit Händen zwingend erforderlich)
https://www.ultraleap.com/product/leap-motion-controller/

### Immersive Wall (Unity-Projekt: GRUNDWASSER_digital_BIGSCREEN)

Die Anwendung kann prinzipiell auf jedem Windows PC mit ausreichender Leistung verwendet werden ist jedeoch für folgende Hardware entwickelt worden:

- Windows 10 Pro, NVIDIA GeForce RTX 3090 mit 24GB, AMD Ryzen 9 16x3950X, 32GB RAM
- Joysticks: 2 x APEM HF45S10U USB
- 3 x 86" 4K-Displays, aufrecht stehend verbunden über nVidia Surround

### Netzwerk

- Die Anwendungen sollten sich im Netzwerk automatisch finden sofern die Netzwerkeinstellungen dies erlauben:
Bei Windows 10 ist das z.b.: Control Panel\System and Security\Windows Defender Firewall\Allowed applications)
- In der Ausstellung sind die Geräte über einen Switch verbunden

## Installation:

Der vollständige Quellcode des Unity Projektes kann bei Senckenberg Museum für Naturkunde Görlitz angefragt werden.
Kontaktinformationen: post-gr@senckenberg.de

### Volumetrisches Display (Unity-Projekt: GRUNDWASSER_digital_VOXON_VX1)

- Unity 2022.1.3f1
- Ultraleap Gemini 5.7.2: https://developer.leapmotion.com/tracking-software-download
- Voxon Unity PlugIn 230201 (unoffizielle Version)
- Keyboard + Maus

Das Unity-Projekt ist vollständig und enthält folgende Packages:

- Leap Motion Core Version 4.9.1
- Leap Motion Examples
- Leap Motion Interaction Engine
- Leap Motion Hands
- Voxon VX1 SDK für Unity: https://voxon.co/sdk-unity/
- Mirror Network Version 57.0.0: https://mirror-networking.com/

### Immersive Wall (Unity-Projekt: GRUNDWASSER_digital_BIGSCREEN)

- Unity 2020.3.23f1

Das Unity-Projekt ist vollständig und enthält folgende Packages:
- Mirror Network Version 57.0.0: https://mirror-networking.com/

## Verwendung:

### Volumetrisches Display (Unity-Projekt: GRUNDWASSER_digital_VOXON_VX1)

Simualtion:
- Objekt greiffen
- Objekt mit zwei Händen zoomen
- Maus hoch und runter schieben um das Auswahlrad zu simulieren (schaltet Modelle weiter)
- Objekte weiterschalten: Tasten "Page up" und "Page down"
- Im Simulationsprogramm für das VX1 können die Tasten W, A, S, D verwendet werden, um die Ansicht zu drehen

Exponat:
- Objekt greiffen
- Objekt mit zwei Händen zoomen
- Auswahlrad drehen um Modelle umzuschalten

### Immersive Wall (Unity-Projekt: GRUNDWASSER_digital_BIGSCREEN)

Simulation: 
- Mit linker Maustaste ins Bild klicken um die Navigation zu aktivieren
- Mit rechter Maustaste klicken, um die Mause wieder zu befreien
- Tasten: W, A, S, D zur Navigation
- Taste: Space = hoch
- Taste: C = runter
- Mausrad: zoomen
- Taste: I = Toggle zwischen normaler Ansicht und stereoskopischer Ansicht (experimentell)

Exponat: 
- Rechter Joystick Achse Horizontal: Kamera links/rechts drehen
- Rechter Joystick Achse Vertikal: Kamera hoch/runter drehen
- Rechter Joystick Achse Rotation: Kamera ein/aus zoomen
- Rechter Joystick Button links: Kamera zoom ein
- Rechter Joystick Button rechts: Kamera zoom aus
- Linker Joystick Achse Horizontal: Fahren vor/zurück
- Linker Joystick Achse Vertikal: Fahren links/rechts
- Linker Joystick Achse Rotation: vertikal auf/ab
- Linker Joystick Button links: vertikal auf
- Linker Joystick Button rechts: vertikal ab

Funktions für Links- und Rechtshänder:
- Alle vier Buttons gleichzeitig gedrückt halten: Vertauschen der Funktionen der Joysticks

## Lizenz:

Dieses Projekt steht unter der Lizenz CC BY 3.0 DE (https://creativecommons.org/licenses/by/3.0/de/)

## Credits:

- Auftraggeber: Senckenberg Gesellschaft für Naturkunde (https://senckenberg.de)
- Entwicklung/Urheber: Lutz Westermann, .hapto GmbH (www.hapto.de, www.vimeo.com/hapto)

## Förderhinweis:

Diese Anwendungen sind Teil des Projektes museum4punkt0 - Digitale Strategien für das Museum der Zukunft, Teilprojekt "Grundwasser digital". Das Projekt museum4punkt0 wird gefördert durch die Beauftragte der Bundesregierung für Kultur und Medien aufgrund eines Beschlusses des Deutschen Bundestages.
Weitere Informationen: www.museum4punkt0.de
