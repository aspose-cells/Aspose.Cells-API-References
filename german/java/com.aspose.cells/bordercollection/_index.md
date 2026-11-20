---
title: "BorderCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Kapselt eine Sammlung von [Border](../../com.aspose.cells/border) Objekten.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Liefert das [Border](../../com.aspose.cells/border)-Element am angegebenen Index. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Liefert die [Color](../../com.aspose.cells/color) der diagonalen Linien. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Liefert den Stil der diagonalen Linien. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Gibt an, ob linke, rechte, obere und untere Rahmen nur auf die äußeren Rahmen eines Zellenbereichs angewendet werden sollen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Setzt die [Color](../../com.aspose.cells/color) aller Rahmen in der Sammlung. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Setzt die [Color](../../com.aspose.cells/color) der diagonalen Linien. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Setzt den Stil der diagonalen Linien. |
| [setOutline(boolean value)](#setOutline-boolean-) | Gibt an, ob linke, rechte, obere und untere Rahmen nur auf die äußeren Rahmen eines Zellenbereichs angewendet werden sollen. |
| [setStyle(int style)](#setStyle-int-) | Setzt den Stil aller Rahmen der Sammlung. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Liefert das [Border](../../com.aspose.cells/border)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Der abzurufende Rahmen. |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


Liefert die [Color](../../com.aspose.cells/color) der diagonalen Linien.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Liefert den Stil der diagonalen Linien.

Siehe [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Gibt an, ob linke, rechte, obere und untere Rahmen nur auf die äußeren Rahmen eines Zellenbereichs angewendet werden sollen. Der Standardwert ist true.

**Remarks**

Funktioniert nur, wenn es auf einen Bereich für bedingte Formatierungen oder Pivot-Tabellen angewendet wird. Wenn false, werden linke, rechte, obere und untere Rahmen auf jede Zelle angewendet, andernfalls nur auf die äußeren Rahmen eines Zellenbereichs. Wenn true, bitte den horizontalen und vertikalen Rahmen der inneren Rahmen des Bereichs für bedingte Formatierungen und Pivot-Tabellen festlegen.

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


Setzt die [Color](../../com.aspose.cells/color) aller Rahmen in der Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Die [Color](../../com.aspose.cells/color) der Rahmen. |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Setzt die [Color](../../com.aspose.cells/color) der diagonalen Linien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Setzt den Stil der diagonalen Linien.

Siehe [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Gibt an, ob linke, rechte, obere und untere Rahmen nur auf die äußeren Rahmen eines Zellenbereichs angewendet werden sollen. Der Standardwert ist true.

**Remarks**

Funktioniert nur, wenn es auf einen Bereich für bedingte Formatierungen oder Pivot-Tabellen angewendet wird. Wenn false, werden linke, rechte, obere und untere Rahmen auf jede Zelle angewendet, andernfalls nur auf die äußeren Rahmen eines Zellenbereichs. Wenn true, bitte den horizontalen und vertikalen Rahmen der inneren Rahmen des Bereichs für bedingte Formatierungen und Pivot-Tabellen festlegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Setzt den Stil aller Rahmen der Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stil der Rahmen |

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

