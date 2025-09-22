# PComp_2025_Richard_Qian_Li


## week 3

I saw in some code "INPUT_PULLUP" was used. It requires connection in another way which took me a while to understand.

I tried to connect 5 buttons to the digital pins that gives me a [five key piano](https://www.youtube.com/shorts/UPWsGzkG6_s)






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
