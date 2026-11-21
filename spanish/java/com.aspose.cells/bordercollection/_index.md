---
title: "BorderCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Encapsula una colección de objetos [Border](../../com.aspose.cells/border).

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
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Obtiene el elemento [Border](../../com.aspose.cells/border) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Obtiene el [Color](../../com.aspose.cells/color) de las líneas diagonales. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Obtiene el estilo de las líneas diagonales. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Indica si los bordes izquierdo, derecho, superior e inferior deben aplicarse solo a los bordes exteriores de un rango de celdas. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Establece el [Color](../../com.aspose.cells/color) de todos los bordes en la colección. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Establece el [Color](../../com.aspose.cells/color) de las líneas diagonales. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Establece el estilo de las líneas diagonales. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indica si los bordes izquierdo, derecho, superior e inferior deben aplicarse solo a los bordes exteriores de un rango de celdas. |
| [setStyle(int style)](#setStyle-int-) | Establece el estilo de todos los bordes de la colección. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Obtiene el elemento [Border](../../com.aspose.cells/border) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). El borde a recuperar. |

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


Obtiene el [Color](../../com.aspose.cells/color) de las líneas diagonales.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Obtiene el estilo de las líneas diagonales.

Ver [CellBorderType](../../com.aspose.cells/cellbordertype).

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


Indica si los bordes izquierdo, derecho, superior e inferior deben aplicarse solo a los bordes exteriores de un rango de celdas. El valor predeterminado es verdadero.

**Remarks**

Solo funciona al aplicarse a un rango para formatos condicionales, tablas dinámicas. Si es falso, los bordes izquierdo, derecho, superior e inferior se aplicarán a cada celda; de lo contrario, solo a los bordes exteriores de un rango de celdas. Si es verdadero, establezca los bordes horizontal y vertical de los bordes internos del rango para formatos condicionales, tablas dinámicas.

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


Establece el [Color](../../com.aspose.cells/color) de todos los bordes en la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Color de los bordes [Color](../../com.aspose.cells/color). |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Establece el [Color](../../com.aspose.cells/color) de las líneas diagonales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Establece el estilo de las líneas diagonales.

Ver [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indica si los bordes izquierdo, derecho, superior e inferior deben aplicarse solo a los bordes exteriores de un rango de celdas. El valor predeterminado es verdadero.

**Remarks**

Solo funciona al aplicarse a un rango para formatos condicionales, tablas dinámicas. Si es falso, los bordes izquierdo, derecho, superior e inferior se aplicarán a cada celda; de lo contrario, solo a los bordes exteriores de un rango de celdas. Si es verdadero, establezca los bordes horizontal y vertical de los bordes internos del rango para formatos condicionales, tablas dinámicas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Establece el estilo de todos los bordes de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de los bordes |

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

