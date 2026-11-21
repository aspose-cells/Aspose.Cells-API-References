---
title: "BorderCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Inkapslar en samling av [Border](../../com.aspose.cells/border) objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Hämtar [Border](../../com.aspose.cells/border)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Hämtar [Color](../../com.aspose.cells/color) för diagonala linjer. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Hämtar stilen för diagonala linjer. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Anger om vänster, höger, övre och nedre kanter ska tillämpas endast på yttre kanter av ett cellområde. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Ställer in [Color](../../com.aspose.cells/color) för alla kanter i samlingen. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Ställer in [Color](../../com.aspose.cells/color) för diagonala linjer. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Ställer in stilen för diagonala linjer. |
| [setOutline(boolean value)](#setOutline-boolean-) | Anger om vänster, höger, övre och nedre kanter ska tillämpas endast på yttre kanter av ett cellområde. |
| [setStyle(int style)](#setStyle-int-) | Ställer in stilen för alla kanter i samlingen. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Hämtar [Border](../../com.aspose.cells/border)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Kanten som ska hämtas. |

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


Hämtar [Color](../../com.aspose.cells/color) för diagonala linjer.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Hämtar stilen för diagonala linjer.

Se [CellBorderType](../../com.aspose.cells/cellbordertype).

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


Anger om vänster, höger, övre och nedre kanter ska tillämpas endast på yttre kanter av ett cellområde. Standardvärdet är true.

**Remarks**

Fungerar endast när den appliceras på ett område för villkorsformatering, pivottabeller. Om false, vänster, höger, övre och nedre kommer att tillämpas på varje cell, annars endast på yttre kanter av ett cellområde. Om true, vänligen ange horisontell och vertikal kant för de inre kanterna i området för villkorsformatering, pivottabeller.

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


Ställer in [Color](../../com.aspose.cells/color) för alla kanter i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Kantens [Color](../../com.aspose.cells/color). |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Ställer in [Color](../../com.aspose.cells/color) för diagonala linjer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Ställer in stilen för diagonala linjer.

Se [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Anger om vänster, höger, övre och nedre kanter ska tillämpas endast på yttre kanter av ett cellområde. Standardvärdet är true.

**Remarks**

Fungerar endast när den appliceras på ett område för villkorsformatering, pivottabeller. Om false, vänster, höger, övre och nedre kommer att tillämpas på varje cell, annars endast på yttre kanter av ett cellområde. Om true, vänligen ange horisontell och vertikal kant för de inre kanterna i området för villkorsformatering, pivottabeller.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Ställer in stilen för alla kanter i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kantens stil |

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

