# Keyword Spotting in Portuguese

This project uses an Arduino Nano 33 BLE Sense to listen to three keywords in Portuguese: "vermelho", "verde" and "azul".

According to the keyword, it turns on the corresponding color in the embedded RGB LED.

## Voice dataset

It has only 50 samples of my own voice.

* https://github.com/fkuhne/KWS-Dataset

## Edge Impulse project

* https://studio.edgeimpulse.com/public/33110/latest

## How to run

1. Open Arduino IDE
2. Add the zip file as a library
3. Go to File->Examples->coursera-kws-arduino Inferencing - Edge Impulse->nano_ble33_sense_microphone_continuous
4. Upload to the board and say the words!
