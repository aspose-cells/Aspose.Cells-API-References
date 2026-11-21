---
title: "Unit"
second_title: "Aspose.Cells for Java API Referansı"
description: "Uzunluk ölçümünü temsil eder"
type: docs
url: /tr/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Uzunluk ölçümünü temsil eder
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Unit()](#Unit--) | varsayılan yapıcı |
| [Unit(double value, int type)](#Unit-double-int-) | Belirtilen çift hassasiyetli kayan nokta sayısı ve UnitType ile Unit yapısının yeni bir örneğini başlatır. |
| [Unit(double value)](#Unit-double-) | Belirtilen çift hassasiyetli kayan nokta sayısı ile Unit yapısının yeni bir örneğini başlatır. |
| [Unit(int value)](#Unit-int-) | Belirtilen 32-bit işaretli tam sayı ile Unit yapısının yeni bir örneğini başlatır. |
| [Unit(String value)](#Unit-java.lang.String-) | Belirtilen uzunluk ile Unit yapısının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | Türüne göre dize al, "px", "pt", "%" vb. değerler alabilir; |
| [Parse(String s)](#Parse-java.lang.String-) | Belirtilen dizeyi bir Unit'e dönüştürür. |
| [Percentage(double n)](#Percentage-double-) | Belirtilen çift hassasiyetli kayan nokta sayısından Yüzde türünde bir Unit oluşturur. |
| [Pixel(int n)](#Pixel-int-) | Belirtilen 32-bit işaretli tam sayıdan Piksel türünde bir Unit oluşturur. |
| [Point(int n)](#Point-int-) | Belirtilen 32-bit işaretli tam sayıdan Nokta türünde bir Unit oluşturur. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Unit'in birim türünü alır. |
| [getValue()](#getValue--) | Unit'in uzunluğunu alır. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Unit'in boş olup olmadığını gösteren bir değeri alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Unit'in dize temsilini al. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


varsayılan yapıcı

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Belirtilen çift hassasiyetli kayan nokta sayısı ve UnitType ile Unit yapısının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |
| tip | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Belirtilen çift hassasiyetli kayan nokta sayısı ile Unit yapısının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Belirtilen 32-bit işaretli tam sayı ile Unit yapısının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Belirtilen uzunluk ile Unit yapısının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


Türüne göre dize al, "px", "pt", "%" vb. değerler alabilir;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tip | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Belirtilen dizeyi bir Unit'e dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Belirtilen çift hassasiyetli kayan nokta sayısından Yüzde türünde bir Unit oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Belirtilen 32-bit işaretli tam sayıdan Piksel türünde bir Unit oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Belirtilen 32-bit işaretli tam sayıdan Nokta türünde bir Unit oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getType() {#getType--}
```
public int getType()
```


Unit'in birim türünü alır.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Unit'in uzunluğunu alır.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Unit'in boş olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```


Unit'in dize temsilini al.

**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

