# ESP32-S3 Touch LCD Demo

- ESP-IDF: 5.5.1
- Target: esp32s3
- Flash size/mode/freq: 16MB / DIO / 80MHz
- Partition: single factory (large) or `partitions.csv`
- Build:
  ```sh
  idf.py set-target esp32s3
  idf.py defconfig
  idf.py build
  idf.py -p COM11 app-flash
  idf.py -p COM11 monitor
