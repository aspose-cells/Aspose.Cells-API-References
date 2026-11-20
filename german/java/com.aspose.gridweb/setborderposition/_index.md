---
title: "SetBorderPosition"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Rahmenposition dar, die für einen Zellenbereich festgelegt werden soll."
type: docs
url: /de/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Stellt die Rahmenposition dar, die für einen Zellenbereich festgelegt werden soll.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Felder

| Feld | Beschreibung |
| --- | --- |
| [BOTTOM](#BOTTOM) | Unterer Rand |
| [CROSS](#CROSS) | Kreuzende Ränder |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Unterer Rand |
| [LEFT](#LEFT) | Linker Rand |
| [NONE](#NONE) | Keine Ränder |
| [OUTLINE](#OUTLINE) | Vertikale Mittelränder |
| [RIGHT](#RIGHT) | Rechter Rand |
| [TOP](#TOP) | Oberer Rand |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | Horizontale Mittelränder |
## Methoden

| Methode | Beschreibung |
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
### BOTTOM {#BOTTOM}
```
public static final int BOTTOM
```


Unterer Rand

### CROSS {#CROSS}
```
public static final int CROSS
```


Kreuzende Ränder

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Unterer Rand

### LEFT {#LEFT}
```
public static final int LEFT
```


Linker Rand

### NONE {#NONE}
```
public static final int NONE
```


Keine Ränder

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


Vertikale Mittelränder

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Rechter Rand

### TOP {#TOP}
```
public static final int TOP
```


Oberer Rand

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


Horizontale Mittelränder

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

