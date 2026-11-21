---
title: "CellValueFormatStrategy"
second_title: "Aspose.Cells för Java API-referens"
description: "Specificerar hur stil ska tillämpas på cellens värde."
type: docs
url: /sv/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

Specificerar hur stil ska tillämpas på cellens värde.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Endast formaterad med cellens ursprungliga stil. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Hämtar den visade strängen i MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Formaterad med cellens visade stil. |
| [NONE](#NONE) | Inte formaterad. |
## Metoder

| Metod | Beskrivning |
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
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


Endast formaterad med cellens ursprungliga stil.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


Hämtar den visade strängen som visas i MS Excel. Huvudskillnaden från [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) är att detta alternativ också beaktar kolumnbreddens effekt. Om kolumnbredden är för liten för att visa den formaterade strängen helt kan "\#" visas, precis som MS Excel gör.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


Formaterad med cellens visade stil.

### NONE {#NONE}
```
public static final int NONE
```


Inte formaterad.

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

