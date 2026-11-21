---
title: "HeaderFooterCommand"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar kommandot för sidhuvud/sidfot."
type: docs
url: /sv/java/com.aspose.cells/headerfootercommand/
---

**Inheritance:**
java.lang.Object
```
public class HeaderFooterCommand
```

Representerar kommandot för sidhuvud/sidfot.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Hämtar teckensnittet för kommandots värde. |
| [getText()](#getText--) | Hämtar texten för kommandot. |
| [getType()](#getType--) | Hämtar header/footer-kommandotypen. |
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
| Parameter | Typ | Beskrivning |
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


Hämtar teckensnittet för kommandots värde.

**Remarks**

Inte användbar för HeaderFooterCommandType.Picture.

**Returns:**
[Font](../../com.aspose.cells/font)
### getText() {#getText--}
```
public String getText()
```


Hämtar texten för kommandot.

**Remarks**

Endast giltig för HeaderFooterCommandType.Text.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Hämtar header/footer-kommandotypen.

Se [HeaderFooterCommandType](../../com.aspose.cells/headerfootercommandtype).

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

