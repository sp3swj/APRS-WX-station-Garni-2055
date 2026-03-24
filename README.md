Stacja pogodowa APRS zbudowana przy wykorzystaniu urządzenia 

Hydrawise Garni 2055 ARCUS

![ba902190f1ad4248ac2cc03eb01fbc54](https://github.com/user-attachments/assets/81e40a49-57ca-4203-8acc-2eecd520e0b7)

=> na bazie plików od SP3VSS i SP3WRO
-> Aktualizacja opisu i testy by SP3SWJ
-> Sprawdzony plik INO i procedura poniżej.

W załączeniu dwa pliki

<img width="290" height="92" alt="image" src="https://github.com/user-attachments/assets/e52e1e94-925a-47f8-b237-16ac57f0c717" />

https://github.com/sp3swj/APRS-WX-station-Garni-2055/blob/main/Garni_WRO_VSS_SWJ_public_2026-03-23.zip

Otwieramy PDF i po kolei...

To po kolei...

Zainstalowałem najnowsze Arduino IDE.

Pobrałem wszystkie biblioteki.

Doinstalowałem obsługę ESP8266 – tekst poniżej wklejamy do „Preferencji” w Arduino:

http://arduino.esp8266.com/stable/package_esp8266com_index.json


<img width="1001" height="540" alt="image" src="https://github.com/user-attachments/assets/313fd2fb-53a4-4fef-bee8-d884d418c06e" />


Opis w załączonym pliku PDF – historia z obrazkami.

Wszystko działa z najnowszymi bibliotekami – nic nie kombinujemy z plikami CFG w źródłach.

Po prostu składamy poprawnie i kompilujemy.

Otwieramy z ZIP załączony plik INO:

**Garni_WRO_VSS_SWJ_public.ino**

Uzupełniamy dane logowania do domowej sieci WiFi.
Wpisujemy znak i hasło APRS-IS.

Włączamy zasilanie GARNI.

Okablowujemy płytkę.

Zasilanie oczywiście z pinów GND oraz 3,3V !!

<img width="305" height="427" alt="image" src="https://github.com/user-attachments/assets/1e727104-adae-4db6-b75a-f822361ebb04" /> <img width="237" height="463" alt="image" src="https://github.com/user-attachments/assets/9584b04d-9d8d-4f8e-9cbb-c9d99ae55a23" /> <img width="533" height="360" alt="image" src="https://github.com/user-attachments/assets/dc5f4e1c-35df-44b7-8a05-59085a06ce16" /> <img width="475" height="468" alt="image" src="https://github.com/user-attachments/assets/552fffe7-d69f-4d0e-8527-e24974cdf965" />

Podłączamy USB do komputera.

Wybieramy poprawny COM w Arduino.
Wybieramy płytkę ESP8266 => NodeMCU 1.0 ESP-12E ESP8266.

Kompilujemy... kilka minut.

Podłączamy Arduino Port Monitor do naszego COM – 115200.

Podglądamy w oknie TXT, czy wszystko się połączyło.
Widzimy adres IP – jeśli poprawnie zalogowało się do WiFi.

<img width="842" height="400" alt="image" src="https://github.com/user-attachments/assets/e9bcf40b-546e-4486-9b4e-47dd88138e5b" />

Wchodzimy na WWW z przeglądarki:

<img width="912" height="507" alt="image" src="https://github.com/user-attachments/assets/1677d181-c627-4ecb-8ecb-abe4ace3a959" />

Czekamy około 15 minut – aż pojawi się na aprs.fi

https://aprs.fi/#!z=11&call=a%2FSP3SWJ-13

<img width="349" height="241" alt="image" src="https://github.com/user-attachments/assets/13ddbc15-566d-487e-bac7-c65bf9b26ace" />

Pozdrawiam – SP3SWJ

/ Dzięki VSS i WRO za pomoc :-)

.
.
.

Poniżej oryginalna zawartość by SP3VSS and SP3WRO

Na linkach:

https://github.com/ArturVSS/APRS-WX-station-Garni-2055

https://github.com/SP3WRO/BresserWeatherSensorBasicAPRS

=========================
Hydrawise Garni 2055 ARCUS
