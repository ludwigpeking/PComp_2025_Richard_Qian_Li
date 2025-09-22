# PComp_2025_Richard_Qian_Li


## week 3

I saw in some code "INPUT_PULLUP" was used. It requires connection in another way which took me a while to understand.
```
    pinMode(buttonPins[i], INPUT_PULLUP);
```

<img width="1755" height="753" alt="5key_piano_PULLUP" src="https://github.com/user-attachments/assets/d60a5ad7-50f7-434f-b25f-b5c748e2b7d3" />



<img width="526" height="567" alt="image" src="https://github.com/user-attachments/assets/88b65abc-abf0-43c6-a478-697323939c3e" />

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
