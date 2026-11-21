---
title: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerlere stil uygulama şeklini belirtir."
type: docs
url: /tr/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerlere stil uygulama şeklini belirtir.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Ayrıştırılan değer basit sayısal/tarih‑zaman değerleri olduğunda stili yerleşik sayı/tarih‑zaman olarak ayarla. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Ayrıştırılan değer için tam özel biçimi ayarla, böylece biçimlendirilmiş değer orijinal girdiyle aynı olur. |
| [NONE](#NONE) | Ayrıştırılan değer için stil ayarlanmaz. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Ayrıştırılan değer basit sayısal/tarih‑zaman değerleri olduğunda stili yerleşik sayı/tarih‑zaman olarak ayarla.

**Remarks**

ms excel, kullanıcının girişi (örneğin CSV dosyası) doğrultusunda tarih‑zaman veya sayısal değerleri ayrıştırdığında, bu değerlerin biçimlendirmesi değişebilir; örneğin sayının baştaki/sondaki sıfırları, tarih‑zamanın yıl/ay/gün sırası gibi. Bu tür, ms excel'in davranışını simüle etmek içindir.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Ayrıştırılan değer için tam özel biçimi ayarla, böylece biçimlendirilmiş değer orijinal girdiyle aynı olur.

### NONE {#NONE}
```
public static final int NONE
```


Ayrıştırılan değer için stil ayarlanmaz.

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

