# Firmware

Current firmware support:

- ArduPilot
- PX4
- Betaflight
- Arduino
- ESP32

Firmware files are located in:

```bash
/firmware
```

---

# Example Arduino Motor Test

```cpp
#include <Servo.h>

Servo esc1;

void setup() {

  Serial.begin(115200);

  esc1.attach(9);

  // Arm ESC
  esc1.writeMicroseconds(1000);

  delay(3000);

  Serial.println("ESC Armed");
}

void loop() {

  Serial.println("Low Speed");
  esc1.writeMicroseconds(1200);
  delay(3000);

  Serial.println("Medium Speed");
  esc1.writeMicroseconds(1400);
  delay(3000);

  Serial.println("Stop");
  esc1.writeMicroseconds(1000);
  delay(3000);
}
```

---

# Recommended Tools

## Hardware

- Soldering iron
- Multimeter
- Heat gun
- Hex drivers
- Wire stripper

## Software

- Fusion 360
- Onshape
- Cura
- Arduino IDE
- Mission Planner
- QGroundControl

---