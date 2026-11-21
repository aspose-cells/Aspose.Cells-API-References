---
title: "DataBar"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe la regla de formato condicional DataBar."
type: docs
url: /es/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Describe la regla de formato condicional DataBar. Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Obtiene el color del eje para celdas con formato condicional como barras de datos. |
| [getAxisPosition()](#getAxisPosition--) | Obtiene la posición del eje de las barras de datos especificadas por una regla de formato condicional. |
| [getBarBorder()](#getBarBorder--) | Obtiene un objeto que especifica el borde de una barra de datos. |
| [getBarFillType()](#getBarFillType--) | Obtiene cómo se rellena una barra de datos con color. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtiene el color de este DataBar. |
| [getDirection()](#getDirection--) | Obtiene la dirección en que se muestra la barra de datos. |
| [getMaxCfvo()](#getMaxCfvo--) | Obtiene el objeto de valor máximo de este DataBar. |
| [getMaxLength()](#getMaxLength--) | Representa la longitud máxima de la barra de datos. |
| [getMinCfvo()](#getMinCfvo--) | Obtiene el objeto de valor mínimo de este DataBar. |
| [getMinLength()](#getMinLength--) | Representa la longitud mínima de la barra de datos. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de barra de datos. |
| [getShowValue()](#getShowValue--) | Obtiene la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Obtiene el color del eje para celdas con formato condicional como barras de datos. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Establece la posición del eje de las barras de datos especificadas por una regla de formato condicional. |
| [setBarFillType(int value)](#setBarFillType-int-) | Establece cómo se rellena una barra de datos con color. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Establece el color de este DataBar. |
| [setDirection(int value)](#setDirection-int-) | Establece la dirección en que se muestra la barra de datos. |
| [setMaxLength(int value)](#setMaxLength-int-) | Representa la longitud máxima de la barra de datos. |
| [setMinLength(int value)](#setMinLength-int-) | Representa la longitud mínima de la barra de datos. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Establece la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Renderiza la barra de datos en la celda a una matriz de bytes de imagen. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Obtiene el color del eje para celdas con formato condicional como barras de datos.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Obtiene la posición del eje de las barras de datos especificadas por una regla de formato condicional.

Ver [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Obtiene un objeto que especifica el borde de una barra de datos.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Obtiene cómo se rellena una barra de datos con color.

Ver [DataBarFillType](../../com.aspose.cells/databarfilltype).

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


Obtiene el color de este DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Obtiene la dirección en que se muestra la barra de datos.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Obtiene el objeto de valor máximo de este DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Representa la longitud máxima de la barra de datos.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Obtiene el objeto de valor mínimo de este DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Representa la longitud mínima de la barra de datos.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de barra de datos.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Obtiene la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. El valor predeterminado es true.

**Returns:**
boolean
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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


Obtiene el color del eje para celdas con formato condicional como barras de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Establece la posición del eje de las barras de datos especificadas por una regla de formato condicional.

Ver [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Establece cómo se rellena una barra de datos con color.

Ver [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Establece el color de este DataBar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Establece la dirección en que se muestra la barra de datos.

Ver [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Representa la longitud máxima de la barra de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Representa la longitud mínima de la barra de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Establece el indicador que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Renderiza la barra de datos en la celda a una matriz de bytes de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Indica la barra de datos en la celda que se debe renderizar |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene algunas propiedades de la imagen de salida |

**Returns:**
byte[] -
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

