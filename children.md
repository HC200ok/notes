Binary: 10110110 <br>
Hex:    b6 <br>
// 读取二进制表示数的每一位 ex：10110110 =》 1，0，1，1，0，1，1，0

```java
// java code
public byte children = 0xb6;
public byte childA;
public byte childB;
public byte childC;
public byte childD;
public byte childE;
public byte childF;
public byte childG;
public byte childH;

public void set(byte children) {
    childA = (byte) (children & 0x01);
    children >>= 1;
    childB = (byte) (children & 0x01);
    children >>= 1;
    childC = (byte) (children & 0x01);
    children >>= 1;
    childD = (byte) (children & 0x01);
    children >>= 1;
    childE = (byte) (children & 0x01);
    children >>= 1;
    childF = (byte) (children & 0x01);
    children >>= 1;
    childG = (byte) (children & 0x01);
    children >>= 1;
    childH = (byte) (children & 0x01);
}
```
