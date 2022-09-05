# Java cheat sheets

### [Maven Standard Directory Layout](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)

---

## Java data types

```java
double dNum = 3.123456789012345; // for storing 15 decimal digits
float fNum = 3.1234567f; // for storing 6 to 7 decimal digits
        
long lNum = 1000; // from -9 223 372 036 854 775 808 to 9 223 372 036 854 775 807
int iX = 123; // from -2 147 483 648 to 2 147 483 647
char cSymb = '#'; // from 0 to 65535 (symbol code)
short sNum = -128; // from -32768 to 32767
byte bNum = -128; // from -128 to 127

boolean bZ = true;
        
String sStr = "some string";
```

![Java types](https://cdn.ttgtmedia.com/rms/onlineImages/server_side-java_primitive_types-f.png)

## Java type conversion

![Java types](https://res.cloudinary.com/xdpiqbx/image/upload/v1651727764/goit/Java/2022-05-05_081448_pnxrj8.png)

---

### Примитивы - хранятся в стеке, ссылочные типы - в куче

---