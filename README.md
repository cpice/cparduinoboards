# Custom ESP32 Boards for Arduino IDE

This repository contains custom ESP32 board definitions for use with the Arduino IDE. It includes multiple boards with different configurations and partition schemes.

## Boards Included
1. **CP ESP32 Module**
   - Based on ESP32 Dev Module.
   - Flash Size: 4MB.
   - Partition Schemes: Default 4MB, 8MB, and 16MB.

2. **CP ESP32C6 Module**
   - Based on ESP32C6 Dev Module.
   - Flash Size: 8MB.
   - Partition Schemes: Default 4MB, 8MB, and 16MB.

3. **CP ESP32 Gateway with PCIE**
   - Based on ARDUINO_LILYGOTPCIE.
   - Flash Size: 16MB.
   - Partition Schemes: Default 4MB, 8MB, and 16MB.

## Partition Schemes
- **cp_partitions_4MB.csv**: Partition scheme for 4MB flash.
- **cp_partitions_8MB.csv**: Partition scheme for 8MB flash.
- **cp_partitions_16MB.csv**: Partition scheme for 16MB flash.

## Installation Instructions
1. Open Arduino IDE.
2. Go to `File > Preferences`.
3. Add the following URL to the "Additional Board Manager URLs" field:
   ```
   https://raw.githubusercontent.com/YourUsername/CustomESP32Boards/main/package_cpboards.json
   ```
4. Click "OK."
5. Go to `Tools > Board > Boards Manager`.
6. Search for `CP ESP32 Platform` and install it.

## Repository Structure
- `boards.txt`: Defines the custom boards.
- `platform.txt`: Platform configuration for the boards.
- `cp_partitions_4MB.csv`: Partition scheme for 4MB flash.
- `cp_partitions_8MB.csv`: Partition scheme for 8MB flash.
- `cp_partitions_16MB.csv`: Partition scheme for 16MB flash.
- `package_cpboards.json`: JSON file for Arduino IDE integration.

## License
This project is licensed under the MIT License.
