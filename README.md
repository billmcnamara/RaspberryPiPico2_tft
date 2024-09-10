# PICO2 Arduino IDE Basic Project: Adafruit ST7735 TFT Display

This project provides a simple example for testing Raspberry Pi Pico 2 (RP2350) compilation and upload using the Arduino IDE, while implementing the Adafruit_ST7735 TFT display library.

## Hardware Setup

To connect a TFT display to the Raspberry Pi Pico 2, use the following pin assignments:

```
#define TFT_CS   17   // Chip Select
#define TFT_RST  16   // Reset
#define TFT_DC   20   // Data/Command
#define TFT_MOSI 19   // Master Out Slave In (SDA)
#define TFT_SCLK 18   // Serial Clock (SCK)
```

![Wiring Diagram](Img/wiring.jpg?raw=true)

## Configuring the Arduino IDE

### 1. Install the Board Manager for Raspberry Pi Pico

- Go to **File -> Preferences** in the Arduino IDE.
- In the **Additional Boards Manager URLs** field, add the following URL:

  ```
  https://github.com/earlephilhower/arduino-pico/releases/download/global/package_rp2040_index.json
  ```

![Preferences Setup](Img/arduino_ide1.jpg?raw=true)

### 2. Select the Raspberry Pi Pico Board

- Open **Tools -> Board -> Board Manager**.
- Search for **Raspberry Pi Pico** and install it from the list.

![Board Manager](Img/arduino_ide2.jpg?raw=true)

## Flashing the Pico

1. Press and hold the "BOOTSEL" button on your Pico2 board.
2. While holding the button, connect the Pico to your computer's USB port.

### Selecting the UF2 Board

- In the Arduino IDE, under **Tools -> Board**, select **UF2_Board**.

![Select Board](Img/arduino_ide3.jpg?raw=true)

### Compile and Upload

1. Once the code is ready, click the **Verify** button to compile your project.
2. Click **Upload** to flash the code to your Pico2.

![Compilation and Upload](Img/arduino_ide4.jpg?raw=true)
