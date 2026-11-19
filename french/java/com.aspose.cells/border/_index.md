---
title: "Bordure"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente la bordure de la cellule."
type: docs
url: /fr/java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

Encapsule l'objet qui représente la bordure de la cellule.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
 
         Style style = cell.getStyle();
         //Set top border style and color
         Border border = style.getBorders().getByBorderType(BorderType.TOP_BORDER);
         border.setLineStyle(CellBorderType.MEDIUM);
         border.setColor(Color.getRed());
         cell.setStyle(style);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Obtient la couleur avec une valeur ARGB sur 32 bits. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient le [Color](../../com.aspose.cells/color) de la bordure. |
| [getLineStyle()](#getLineStyle--) | Obtient le type de bordure de cellule. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur de thème de la bordure. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Définit la couleur avec une valeur ARGB sur 32 bits. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Définit le [Color](../../com.aspose.cells/color) de la bordure. |
| [setLineStyle(int value)](#setLineStyle-int-) | Définit le type de bordure de cellule. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur de thème de la bordure. |
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Obtient la couleur avec une valeur ARGB sur 32 bits.

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


Obtient le [Color](../../com.aspose.cells/color) de la bordure.

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


Obtient le type de bordure de cellule.

Voir [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtient la couleur de thème de la bordure.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Définit la couleur avec une valeur ARGB sur 32 bits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Définit le [Color](../../com.aspose.cells/color) de la bordure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


Définit le type de bordure de cellule.

Voir [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Définit la couleur de thème de la bordure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

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

