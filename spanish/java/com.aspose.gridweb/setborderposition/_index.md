---
title: "SetBorderPosition"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la posición del borde que se debe establecer de un rango de celdas."
type: docs
url: /es/java/com.aspose.gridweb/setborderposition/
---

**Inheritance:**
java.lang.Object
```
public final class SetBorderPosition
```

Representa la posición del borde que se debe establecer de un rango de celdas.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, GridWeb1.getWorkSheets().get(0).getCells().get(0, 0).getStyle().getLeftBorderStyle());
```
## Campos

| Campo | Descripción |
| --- | --- |
| [BOTTOM](#BOTTOM) | Borde inferior |
| [CROSS](#CROSS) | Bordes cruzados |
| [HORIZONTAL_MIDDLE](#HORIZONTAL-MIDDLE) | Borde inferior |
| [LEFT](#LEFT) | Borde izquierdo |
| [NONE](#NONE) | Sin bordes |
| [OUTLINE](#OUTLINE) | Bordes VerticalMiddle |
| [RIGHT](#RIGHT) | Borde derecho |
| [TOP](#TOP) | Borde superior |
| [VERTICAL_MIDDLE](#VERTICAL-MIDDLE) | Bordes HorizontalMiddle |
## Métodos

| Método | Descripción |
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


Borde inferior

### CROSS {#CROSS}
```
public static final int CROSS
```


Bordes cruzados

### HORIZONTAL_MIDDLE {#HORIZONTAL-MIDDLE}
```
public static final int HORIZONTAL_MIDDLE
```


Borde inferior

### LEFT {#LEFT}
```
public static final int LEFT
```


Borde izquierdo

### NONE {#NONE}
```
public static final int NONE
```


Sin bordes

### OUTLINE {#OUTLINE}
```
public static final int OUTLINE
```


Bordes VerticalMiddle

### RIGHT {#RIGHT}
```
public static final int RIGHT
```


Borde derecho

### TOP {#TOP}
```
public static final int TOP
```


Borde superior

### VERTICAL_MIDDLE {#VERTICAL-MIDDLE}
```
public static final int VERTICAL_MIDDLE
```


Bordes HorizontalMiddle

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

