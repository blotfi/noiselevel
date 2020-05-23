## Noise Level
Programme pour ESP32 qui récupère les informations sonores via l'interface I2S du microphone MEMS INMP441

Affiche sur un écran TFT 2.4" 320*240 ILI 9341, la FFT temps réel du signal sous forme de 9 barres et le niveau de puissance global

le code requiert les **bibliothèques** :

    arduinoFFT
    MiniGrafx + font ArialRounded (mais on peut utiliser une autre)
    ILI9341_SPI

#### Connexions

    // GPIO2            pin 5 TFT_DC    
    // GPIO22           -               
    // GPIO16   RXD2    -               
    // GPIO17   TXD2    -               
    // GPIO18   SCK     pin 7 TFT_SCK   
    // GPIO19   MISO    pin 9 TFT_SDO   
    // GPIO23   MOSI    pin 6 TFT_SDI   
    // GPIO15           pin 3 TFT_CS    
    // GPI03    RXD0    -               
    // GPIO1    TXD0    -               
    // GPIO34   -       -               
    // GPIO35   -       -               
    // GPIO25   -                       
    // GPIO26   -       pin 8 TFT_LED   
    // GPIO27   -       INMP441_WS               
    // GPIO14           INMP441_SCK               
    // GPIO32           INMP441_SD               
    // -------  ------  --------------- 
    // GND      -       pin 2 TFT_GND   
    // VCC 5 V  -                       
    // VCC 5 V  -                       
    // EN       -       pin 4 TFT_RST   
    // 3.3V             pin 1 TFT_VDD

![proto1](/noise_bb.png)  ![proto2](/noisefft.jpeg)
 
