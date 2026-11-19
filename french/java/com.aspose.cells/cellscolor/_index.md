---
title: "CellsColor"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les types de couleur."
type: docs
url: /fr/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Représente tous les types de couleur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Obtient la couleur à partir d'une valeur ARGB 32 bits. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient la couleur RVB. |
| [getColorIndex()](#getColorIndex--) | Obtient l'index de couleur dans la palette de couleurs. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur du thème. |
| [getTransparency()](#getTransparency--) | Obtient la transparence sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [getType()](#getType--) | Le type de couleur. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Obtient la couleur qui doit être appliquée à la cellule ou à la forme. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Définit la couleur à partir d'une valeur ARGB 32 bits. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Définit la couleur RVB. |
| [setColorIndex(int value)](#setColorIndex-int-) | Définit l'index de couleur dans la palette de couleurs. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Définit la couleur qui doit être appliquée à la cellule ou à la forme. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Obtient la couleur du thème. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Définir la teinte de la couleur de la forme |
| [setTransparency(double value)](#setTransparency-double-) | Définit la transparence sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgb() {#getArgb--}
```
public int getArgb()
```


Obtient la couleur à partir d'une valeur ARGB 32 bits.

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


Obtient la couleur RVB.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Obtient l'index de couleur dans la palette de couleurs. S'applique uniquement aux couleurs indexées.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtient la couleur du thème. S'applique uniquement au type de couleur du thème.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Obtient la transparence sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Le type de couleur.

Voir [ColorType](../../com.aspose.cells/colortype).

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


Obtient la couleur qui doit être appliquée à la cellule ou à la forme.

**Remarks**

L'expression de la couleur de la cellule et de la forme est différente. Par exemple, la couleur du thème avec la même valeur de teinte ne sera pas identique dans la cellule et la forme.

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


Définit la couleur à partir d'une valeur ARGB 32 bits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Définit la couleur RVB.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Définit l'index de couleur dans la palette de couleurs. S'applique uniquement aux couleurs indexées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Définit la couleur qui doit être appliquée à la cellule ou à la forme.

**Remarks**

L'expression de la couleur de la cellule et de la forme est différente. Par exemple, la couleur du thème avec la même valeur de teinte ne sera pas identique dans la cellule et la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Obtient la couleur du thème. S'applique uniquement au type de couleur du thème.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Définir la teinte de la couleur de la forme

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Définit la transparence sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

