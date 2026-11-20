---
title: "BorderCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Incapsula una raccolta di oggetti [Border](../../com.aspose.cells/border).

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Ottiene l'elemento [Border](../../com.aspose.cells/border) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Ottiene il [Color](../../com.aspose.cells/color) delle linee diagonali. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Ottiene lo stile delle linee diagonali. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Indica se i bordi sinistro, destro, superiore e inferiore devono essere applicati solo ai bordi esterni di un intervallo di celle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) di tutti i bordi nella raccolta. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) delle linee diagonali. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Imposta lo stile delle linee diagonali. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indica se i bordi sinistro, destro, superiore e inferiore devono essere applicati solo ai bordi esterni di un intervallo di celle. |
| [setStyle(int style)](#setStyle-int-) | Imposta lo stile di tutti i bordi della raccolta. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Ottiene l'elemento [Border](../../com.aspose.cells/border) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Il bordo da recuperare. |

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


Ottiene il [Color](../../com.aspose.cells/color) delle linee diagonali.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Ottiene lo stile delle linee diagonali.

Vedi [CellBorderType](../../com.aspose.cells/cellbordertype).

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


Indica se i bordi sinistro, destro, superiore e inferiore devono essere applicati solo ai bordi esterni di un intervallo di celle. Il valore predefinito è true.

**Remarks**

Funziona solo quando viene applicato a un intervallo per formattazioni condizionali, tabelle pivot. Se false, i bordi sinistro, destro, superiore e inferiore verranno applicati a ciascuna cella, altrimenti solo ai bordi esterni di un intervallo di celle. Se true, impostare i bordi orizzontali e verticali dei bordi interni dell'intervallo per formattazioni condizionali, tabelle pivot.

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


Imposta il [Color](../../com.aspose.cells/color) di tutti i bordi nella raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Il [Color](../../com.aspose.cells/color) dei bordi. |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Imposta il [Color](../../com.aspose.cells/color) delle linee diagonali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Imposta lo stile delle linee diagonali.

Vedi [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indica se i bordi sinistro, destro, superiore e inferiore devono essere applicati solo ai bordi esterni di un intervallo di celle. Il valore predefinito è true.

**Remarks**

Funziona solo quando viene applicato a un intervallo per formattazioni condizionali, tabelle pivot. Se false, i bordi sinistro, destro, superiore e inferiore verranno applicati a ciascuna cella, altrimenti solo ai bordi esterni di un intervallo di celle. Se true, impostare i bordi orizzontali e verticali dei bordi interni dell'intervallo per formattazioni condizionali, tabelle pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Imposta lo stile di tutti i bordi della raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stile dei bordi |

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

