---
title: "SetBorderPosition"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la posizione del bordo da impostare per un intervallo di celle."
type: docs
url: /it/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Rappresenta la posizione del bordo da impostare per un intervallo di celle.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Campi

| Campo | Descrizione |
| --- | --- |
| [BOTTOM](#BOTTOM) | Bordo inferiore |
| [CROSS](#CROSS) | Bordi incrociati |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Bordo inferiore |
| [LEFT](#LEFT) | Bordo sinistro |
| [NONE](#NONE) | Nessun bordo |
| [OUTLINE](#OUTLINE) | Bordi VerticalMiddle |
| [RIGHT](#RIGHT) | Bordo destro |
| [TOP](#TOP) | Bordo superiore |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | Bordi HorizontalMiddle |
## Metodi

| Metodo | Descrizione |
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


Bordo inferiore

### CROSS {#CROSS}
```
public static final int CROSS
```


Bordi incrociati

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Bordo inferiore

### LEFT {#LEFT}
```
public static final int LEFT
```


Bordo sinistro

### NONE {#NONE}
```
public static final int NONE
```


Nessun bordo

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


Bordi VerticalMiddle

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Bordo destro

### TOP {#TOP}
```
public static final int TOP
```


Bordo superiore

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


Bordi HorizontalMiddle

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

