# LilyGO T-Display S3

## Diagrams

![lilygo_tdisplay_s3.jpg.png](images/lilygo_tdisplay_s3.jpg.png){w=600px align=center}

## Enable Display

```c++
void setup() {
 pinMode(15, OUTPUT);
 digitalWrite(15, HIGH);
}
```

## Brightness

```cpp
const int ledPin = 38;  
const int freq = 5000;  
const int ledChannel = 0;  
const int resolution = 8;  

void setup() {
 ledcSetup(ledChannel, freq, resolution);  
 ledcAttachPin(ledPin, ledChannel);  
 ledcWrite(ledChannel, 25);  // 0-255
}
```

## References

- <https://github.com/Xinyuan-LilyGO/T-Display-S3/>
