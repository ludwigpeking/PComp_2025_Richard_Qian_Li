# PComp_2025_Richard_Qian_Li

## week 1
I am thrilled to finally have the chance to explore some hardware skills, which I never tried on.

- I installed the Ardurino IDE, and installed libraries like WiFiNINA, LSM6DS3, RTCZero, BLE 

- I tried to manipulte the arguments in this snippets that gives me urging LED Flash effects.
```cpp
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
  static int delayTime = 2000; 
  digitalWrite(LED_BUILTIN, HIGH);
  delay(delayTime);
  digitalWrite(LED_BUILTIN, LOW);
  delay(delayTime);

  if (delayTime > 150) {
    delayTime /= 1.4; 
  }
  else {
    delayTime = 150;
  }
}
```

- I tried plug the controller to my computer via micro USB

- Learned the names of the parts