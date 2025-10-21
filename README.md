# ESP32-S3 Round Touch LCD Demo 360x360

A version of the waveshare demo project for the https://www.waveshare.com/product/arduino/displays/lcd-spi-qspi/esp32-s3-touch-lcd-1.85.htm?sku=28514 esp32 round display with all build errors fixed.

This builds with VS Code using the Espressif ESP-IDF extension with parameters below.

- ESP-IDF: 5.5.1
- Target: esp32s3
- Flash size/mode/freq: 16MB / DIO / 80MHz
- Partition: single factory (large) 
- Build:
  ```sh
  idf.py set-target esp32s3
  idf.py defconfig
  idf.py build
  idf.py -p COMXX app-flash
  idf.py -p COMXX monitor
