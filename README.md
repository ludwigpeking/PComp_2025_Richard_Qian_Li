# PComp_2025_Richard_Qian_Li

## week 4

<img width="2388" height="1668" alt="Weixin Image_20250930152239_17_2" src="https://github.com/user-attachments/assets/ff0187a7-260c-4ce4-b9ab-2689df420c29" />

![FBNN0RKGPBD4JQV](https://github.com/user-attachments/assets/3c7ee525-8506-43af-a50a-6f7823378fcb)

![FDWXHH8GPLJ13WT](https://github.com/user-attachments/assets/5171cc08-f935-4905-84b1-370958f8d229)

## week 3

I saw in some code "INPUT_PULLUP" was used. It requires connection in another way which took me a while to understand.
```
    pinMode(buttonPins[i], INPUT_PULLUP);
```

<img width="1755" height="753" alt="5key_piano_PULLUP" src="https://github.com/user-attachments/assets/d60a5ad7-50f7-434f-b25f-b5c748e2b7d3" />



<img width="526" height="567" alt="image" src="https://github.com/user-attachments/assets/88b65abc-abf0-43c6-a478-697323939c3e" />

I tried to connect 5 buttons to the digital pins that gives me a [VIDEO: five key piano](https://www.youtube.com/shorts/UPWsGzkG6_s)
You can play songs with only 5 notes like À la Claire Fontaine all right with it.
Since we are a school of the arts, it has to do more than that. So we can change the note map to make it other pentatonic music, like: Amazing Grace, or the Jasmine Flower.
```
// Musical notes for each button (C5, D5, E5, G5, A5)
const int notes[] = {
  NOTE_C5,  // D7 button
  NOTE_D5,  // D6 button  
  NOTE_E5,  // D5 button
  NOTE_G5,  // D4 button
  NOTE_A5   // D3 button
};
```
[Video : A pentagonic piano ]( https://www.youtube.com/shorts/3a1f_Sgb6Dc)




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
