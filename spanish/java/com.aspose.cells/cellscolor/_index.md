---
title: "CellsColor"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todos los tipos de color."
type: docs
url: /es/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Representa todos los tipos de color.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Obtiene el color a partir de un valor ARGB de 32 bits. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtiene el color RGB. |
| [getColorIndex()](#getColorIndex--) | Obtiene el índice de color en la paleta de colores. |
| [getThemeColor()](#getThemeColor--) | Obtiene el color del tema. |
| [getTransparency()](#getTransparency--) | Obtiene la transparencia como un valor de 0.0 (opaco) a 1.0 (claro). |
| [getType()](#getType--) | El tipo de color. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Obtiene el color que debe aplicarse a la celda o forma. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Establece el color a partir de un valor ARGB de 32 bits. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Establece el color RGB. |
| [setColorIndex(int value)](#setColorIndex-int-) | Establece el índice de color en la paleta de colores. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Establece el color que debe aplicarse a la celda o forma. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Obtiene el color del tema. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Establece el tono del color de la forma |
| [setTransparency(double value)](#setTransparency-double-) | Establece la transparencia como un valor de 0.0 (opaco) a 1.0 (claro). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


Obtiene el color a partir de un valor ARGB de 32 bits.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Obtiene el color RGB.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Obtiene el índice de color en la paleta de colores. Solo se aplica a colores indexados.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtiene el color del tema. Solo se aplica al tipo de color de tema.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Obtiene la transparencia como un valor de 0.0 (opaco) a 1.0 (claro).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


El tipo de color.

Ver [ColorType](../../com.aspose.cells/colortype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


Obtiene el color que debe aplicarse a la celda o forma.

**Remarks**

La expresión del color de la celda y la forma es diferente. Por ejemplo: el color del tema con el mismo valor de tono no será el mismo en la celda y la forma.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


Establece el color a partir de un valor ARGB de 32 bits.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Establece el color RGB.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Establece el índice de color en la paleta de colores. Solo se aplica a colores indexados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Establece el color que debe aplicarse a la celda o forma.

**Remarks**

La expresión del color de la celda y la forma es diferente. Por ejemplo: el color del tema con el mismo valor de tono no será el mismo en la celda y la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Obtiene el color del tema. Solo se aplica al tipo de color de tema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Establece el tono del color de la forma

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Establece la transparencia como un valor de 0.0 (opaco) a 1.0 (claro).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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

