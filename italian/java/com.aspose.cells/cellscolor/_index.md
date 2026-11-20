---
title: "CellsColor"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutti i tipi di colore."
type: docs
url: /it/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Rappresenta tutti i tipi di colore.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Restituisce il colore da un valore ARGB a 32 bit. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Restituisce il colore RGB. |
| [getColorIndex()](#getColorIndex--) | Restituisce l'indice del colore nella tavolozza dei colori. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getTransparency()](#getTransparency--) | Restituisce la trasparenza come valore da 0.0 (opaco) attraverso 1.0 (trasparente). |
| [getType()](#getType--) | Il tipo di colore. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Restituisce il colore da applicare alla cella o alla forma. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Imposta il colore da un valore ARGB a 32 bit. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Imposta il colore RGB. |
| [setColorIndex(int value)](#setColorIndex-int-) | Imposta l'indice del colore nella tavolozza dei colori. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Imposta il colore da applicare alla cella o alla forma. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Ottiene il colore del tema. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Imposta la tinta del colore della forma |
| [setTransparency(double value)](#setTransparency-double-) | Imposta la trasparenza come valore da 0.0 (opaco) attraverso 1.0 (trasparente). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


Restituisce il colore da un valore ARGB a 32 bit.

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


Restituisce il colore RGB.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Restituisce l'indice del colore nella tavolozza dei colori. Si applica solo ai colori indicizzati.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Restituisce il colore del tema. Si applica solo al tipo di colore del tema.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Restituisce la trasparenza come valore da 0.0 (opaco) attraverso 1.0 (trasparente).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Il tipo di colore.

Vedi [ColorType](../../com.aspose.cells/colortype).

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


Restituisce il colore da applicare alla cella o alla forma.

**Remarks**

L'espressione del colore della cella e della forma è diversa. Per esempio: il colore del tema con lo stesso valore di tinta non sarà lo stesso nella cella e nella forma.

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


Imposta il colore da un valore ARGB a 32 bit.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Imposta il colore RGB.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Imposta l'indice del colore nella tavolozza dei colori. Si applica solo ai colori indicizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Imposta il colore da applicare alla cella o alla forma.

**Remarks**

L'espressione del colore della cella e della forma è diversa. Per esempio: il colore del tema con lo stesso valore di tinta non sarà lo stesso nella cella e nella forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Restituisce il colore del tema. Si applica solo al tipo di colore del tema.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Imposta la tinta del colore della forma

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tinta | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Imposta la trasparenza come valore da 0.0 (opaco) attraverso 1.0 (trasparente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

