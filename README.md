# Weather_lib
![image](https://user-images.githubusercontent.com/87471423/127824947-1dca7def-fa95-4721-a362-bd008ab2ed69.png)

Bildquelle: https://de.wikipedia.org/wiki/OpenWeatherMap#/media/Datei:OpenWeather-Logo.jpg\n
Eine Bibliothek um aktuelle Wetter Daten auszulesen


## Funktionen:
    o Herausfinden der aktuellen Wetterlage eines stantortes
    o Einfache anwendung durch get_item() Funktion
    o Korrekte und präziese angabe von Warnungen und Fehlern bei verwendung des Codes
    o Zurückgabe in verschiedenen Einheiten 
      Windgeschwindigkeit: (km/h, mp/h)
      Temperatur:          (°C, °F, °K)
 
 ## Benötigte Librarys:
     o inspect:   -> Für genaue angabe der Zeile, aus der die Warnung oder der Error entspringt
                  -> pip install inspect
     o termcolor: -> Um Warnungen in einer anderen Farbe, als Fehler hervorzuheben
                  -> pip install termcolor
     o pyowm:     -> Für den erhalt der Wetterdaten aus allen Regionen der Welt
                  -> pip install pyowm (API key erforderlich Link: https://openweathermap.org/api
     o sys:       -> Angabe der Errors mit file=sys.stderr
                  -> pip install sys 
 
 ## Verwendung:
     -> Einfach starten der main Funktion im File: weather.py um einen einblick in die vielen Funktionen
        und Features der Library zu erhalten
     
     Main:
     def main():
    """

    It is to test the program
    """
    w = Weather('Madrid')
    item = w.get_item('temperature', 'feels_like', 'celsius')
    print('Weather_data: ', item)
 
