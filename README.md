# AWTRIX Sensor-Anzeige (Home Assistant Blueprint)

Zeigt einen beliebigen Home-Assistant-Sensor als eigene App auf einem
[AWTRIX NG](https://blueforcer.github.io/awtrix-ng/) Pixel-Panel an –
direkt per MQTT, ohne Berry-App oder Statestream. Aktualisiert sich
automatisch bei jeder Sensor-Änderung.

## Funktionen

- AWTRIX-Panel per Geräte-Dropdown auswählen, kein manuelles MQTT-Topic
- Textfarbe mit Schwellenwerten (z. B. grün/orange/blau je nach Wert)
- Laufschrift-Feinsteuerung (Modus, Tempo, Richtung, Einstieg, Pause)
- Hintergrundeffekt und Wetter-Overlay
- Fortschrittsbalken für Prozentwerte
- Automatisches Ausblenden bei veralteten Sensorwerten
- Optional: geräteweiter App-Übergang mitsetzen

## Installation

In Home Assistant: **Einstellungen → Automatisierungen → Blueprints →
Blueprint importieren**, dann diese URL einfügen:

```
https://raw.githubusercontent.com/Heronidas/ha-awtrix_ng-sensor-display/main/awtrix_sensor.yaml
```

Danach unter **Automatisierung erstellen → aus Blueprint** die
"AWTRIX Sensor-Anzeige" auswählen und die Felder ausfüllen.

## Voraussetzungen

- AWTRIX NG Firmware (nicht AWTRIX 3 – andere API)
- MQTT-Broker, mit dem AWTRIX verbunden ist
- Home-Assistant-MQTT-Discovery für das AWTRIX-Gerät aktiv (für die
  Geräteauswahl im Blueprint)

## Lizenz

Frei nutzbar und anpassbar.
