---
title: "HeaderFooterCommand"
second_title: "Aspose.Cells for Java API Referansı"
description: "Üst bilgi/alt bilgi komutunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/headerfootercommand/
---

**Inheritance:**
java.lang.Object
```
public class HeaderFooterCommand
```

Üst bilgi/alt bilgi komutunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Komutun değerinin yazı tipini alır. |
| [getText()](#getText--) | Komutun metnini alır. |
| [getType()](#getType--) | Üstbilgi/altbilgi komut tipini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getFont() {#getFont--}
```
public Font getFont()
```


Komutun değerinin yazı tipini alır.

**Remarks**

HeaderFooterCommandType.Picture için işe yaramaz.

**Returns:**
[Font](../../com.aspose.cells/font)
### getText() {#getText--}
```
public String getText()
```


Komutun metnini alır.

**Remarks**

Yalnızca HeaderFooterCommandType.Text için geçerlidir.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Üstbilgi/altbilgi komut tipini alır.

Bakın [HeaderFooterCommandType](../../com.aspose.cells/headerfootercommandtype).

**Returns:**
int
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

