---
title: "SignificantDigitsType"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sayısal değerlerin çıktısı için anlamlı basamak türünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Sayısal değerlerin çıktısı için anlamlı basamak türünü temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15 basamak |
| [G_17](#G-17) | 17 basamak, değeri "G17" ile biçimlendirerek. |
| [ROUNDING_17](#ROUNDING-17) | 17 basamak, değeri yuvarlayarak. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15 basamak

### G_17 {#G-17}
```
public static final int G_17
```


17 basamak, değeri "G17" ile biçimlendirerek.

**Remarks**

Bazı double değerleri için "G17", kullanıcı tarafından girilen orijinal/gerçek değerden farklı bir değer verebilir. Örneğin, double değer 0.15 çıktıda 0.14999999999999999 olarak; double değer 1.0E-16 çıktıda 9.9999999999999998E-17 olarak gösterilir. Ms Excel bu değerleri tutarsız şekilde işler; 0.15'i xlsx dosyasında 0.15 olarak kaydeder, ancak 1.0E-16 için kaydedilen değer xlsx dosyasında 9.9999999999999998E-17'dir.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17 basamak, değeri yuvarlayarak.

**Remarks**

Bu tür genellikle değeri, kullanıcı tarafından girilen orijinal/gerçek değer olarak çıktılar. 0.15 için "0.15", 1.0E-16 için ise "1.0E-16" üretir. Ancak bazı özel durumlar, gerçek değerden farklı değerler verebilir. Örneğin, 208435494.96478021 sayısını 17 basamağa ("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#") yuvarladığınızda çıktı 208435494.96478 olur.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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

