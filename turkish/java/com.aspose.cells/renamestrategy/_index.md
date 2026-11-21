---
title: "RenameStrategy"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sütunların yinelenen adları için strateji seçeneği."
type: docs
url: /tr/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Sütunların yinelenen adları için strateji seçeneği.

**Remarks**

Başlıklarla veri işlenirken, bazı senaryolar tüm sütunlar için başlıkların tekrarlanmamasını gerektirir. Örneğin, verileri bir veri tablosuna dışa aktarırken ve başlığın veri tablosunun sütun adı olarak alınması gerektiğinde, başlığın yinelenen değerleri geçersizdir. Bu tür durumlarda, kullanıcı bu stratejiyi belirterek nasıl ele alacağını belirleyebilir.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [DIGIT](#DIGIT) | Rakamla adlandırıldı. |
| [EXCEPTION](#EXCEPTION) | İstisna fırlatır. |
| [LETTER](#LETTER) | Harfle adlandırıldı.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Rakamla adlandırıldı. Yinelenen adlar ...1, ...2, vb. şeklinde olur.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


İstisna fırlatır.

### LETTER {#LETTER}
```
public static final int LETTER
```


Harfle adlandırıldı.. Yinelenen adlar ...A, ...B, vb. şeklinde olur.

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

