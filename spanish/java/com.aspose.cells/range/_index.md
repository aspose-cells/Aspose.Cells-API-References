---
title: "Range"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Encapsula el objeto que representa un rango de celdas dentro de una hoja de cálculo.

**Remarks**

La clase Range denota una región de la hoja de cálculo de Excel. Con ella, puedes dar formato y establecer el valor del rango. Y también puedes copiar fácilmente un rango de Excel.

**Example**

El siguiente ejemplo muestra cómo crear un rango y establecer el valor del rango en Excel.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Constructor de la clase. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Constructor de la clase. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica formatos a todo un rango. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Rellena automáticamente el rango objetivo. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Rellena automáticamente el rango objetivo. |
| [clear()](#clear--) | Limpia este rango. |
| [clearComments()](#clearComments--) | Limpia los comentarios de este rango. |
| [clearContents()](#clearContents--) | Limpia el contenido de este rango. |
| [clearFormats()](#clearFormats--) | Limpia los formatos de este rango. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Solo elimina hipervínculos. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc., desde un rango de origen. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Copiando el rango con opciones de pegado especial. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Copia datos de celdas (incluidas fórmulas) desde un rango de origen. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Copia la configuración de estilo de un rango de origen. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Copia el valor de la celda de un rango de origen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Obtiene el objeto [Cell](../../com.aspose.cells/cell) en este rango. |
| [getAddress()](#getAddress--) | Obtiene la dirección del rango. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Obtiene el objeto [Cell](../../com.aspose.cells/cell) o null en este rango. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Obtiene la cantidad de columnas en el rango. |
| [getColumnWidth()](#getColumnWidth--) | Establece u obtiene el ancho de columna de este rango |
| [getCurrentRegion()](#getCurrentRegion--) | Devuelve un objeto Range que representa la región actual. |
| [getEntireColumn()](#getEntireColumn--) | Obtiene un objeto Range que representa la columna completa (o columnas) que contiene el rango especificado. |
| [getEntireRow()](#getEntireRow--) | Obtiene un objeto Range que representa la fila completa (o filas) que contiene el rango especificado. |
| [getFirstColumn()](#getFirstColumn--) | Obtiene el índice de la primera columna del rango. |
| [getFirstRow()](#getFirstRow--) | Obtiene el índice de la primera fila del rango. |
| [getHeight()](#getHeight--) | Obtiene el ancho de un rango en puntos. |
| [getHyperlinks()](#getHyperlinks--) | Obtiene todos los hipervínculos en el rango. |
| [getLeft()](#getLeft--) | Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango. |
| [getName()](#getName--) | Obtiene el nombre del rango. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Obtiene el [Range](../../com.aspose.cells/range) por desplazamiento. |
| [getRefersTo()](#getRefersTo--) | Obtiene a qué se refiere el rango. |
| [getRowCount()](#getRowCount--) | Obtiene la cantidad de filas en el rango. |
| [getRowHeight()](#getRowHeight--) | Establece u obtiene la altura de las filas en este rango |
| [getTop()](#getTop--) | Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango. |
| [getValue()](#getValue--) | Obtiene el valor del rango. |
| [getWidth()](#getWidth--) | Obtiene el ancho de un rango en puntos. |
| [getWorksheet()](#getWorksheet--) | Obtiene el objeto [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) que contiene este rango. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Devuelve un objeto [Range](../../com.aspose.cells/range) que representa la intersección rectangular de dos rangos. |
| [isBlank()](#isBlank--) | Indica si el rango contiene valores. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Indica si el rango se intersecta. |
| [iterator()](#iterator--) | Obtiene el enumerador de celdas en este Range. |
| [merge()](#merge--) | Combina un rango de celdas en una sola celda. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Mueve el rango actual al rango de destino. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Introduce un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Establece u obtiene el ancho de columna de este rango |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Establece los bordes internos del rango. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre del rango. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Establece el borde de contorno alrededor de un rango de celdas. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Establece el borde de contorno alrededor de un rango de celdas. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Establece los bordes externos alrededor de un rango de celdas. |
| [setRowHeight(double value)](#setRowHeight-double-) | Establece u obtiene la altura de las filas en este rango |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Establece el estilo del rango. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Aplica el estilo de la celda. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor del rango. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Convierte el rango a HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Convierte el rango a imagen. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Convierte el rango a valor JSON. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Range actual. |
| [transpose()](#transpose--) | Transpone (rota) datos de filas a columnas o viceversa. |
| [unMerge()](#unMerge--) | Descombina celdas combinadas de este rango. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Devuelve la unión de dos rangos. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Devuelve el resultado de la unión de dos rangos. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Devuelve el resultado de la unión de dos rangos. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Constructor de la clase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Constructor de la clase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (base cero) |
| rowNumber | int | Número de filas (basado en uno) |
| columnNumber | int | Número de columnas (basado en uno) |
| cells | [Cells](../../com.aspose.cells/cells) | El objeto Range pertenece a este objeto Cells. |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Agrega un hipervínculo a una celda especificada o a un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | Dirección del hipervínculo. |
| textToDisplay | java.lang.String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | java.lang.String | El texto de screenTip para el hipervínculo especificado. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Aplica formatos a todo un rango.

**Remarks**

Cada celda en este rango contendrá un objeto [Style](../../com.aspose.cells/style). Por lo tanto, este es un método que consume mucha memoria. Por favor, úselo con cuidado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto de estilo que se aplicará. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Banderas que indican las propiedades de formato aplicadas. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Rellena automáticamente el rango objetivo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | el rango objetivo. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Rellena automáticamente el rango objetivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | El rango targed. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). El tipo de auto relleno. |

### clear() {#clear--}
```
public void clear()
```


Limpia este rango.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Limpia los comentarios de este rango.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Limpia el contenido de este rango.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Limpia los formatos de este rango.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Solo elimina hipervínculos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clearFormat | boolean | Indica si se debe borrar el formato de los hipervínculos. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc., desde un rango de origen.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objeto [Range](../../com.aspose.cells/range) de origen. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Copiando el rango con opciones de pegado especial.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango de origen. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Las opciones de pegado especial. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Copia datos de celdas (incluidas fórmulas) desde un rango de origen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objeto [Range](../../com.aspose.cells/range) de origen. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Copia la configuración de estilo de un rango de origen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objeto [Range](../../com.aspose.cells/range) de origen. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Copia el valor de la celda de un rango de origen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objeto [Range](../../com.aspose.cells/range) de origen. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Obtiene el objeto [Cell](../../com.aspose.cells/cell) en este rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | int | Desplazamiento de columna en este rango, basado en cero. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Obtiene la dirección del rango.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Obtiene el objeto [Cell](../../com.aspose.cells/cell) o null en este rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | int | Desplazamiento de columna en este rango, basado en cero. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Obtiene la cantidad de columnas en el rango.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Establece u obtiene el ancho de columna de este rango

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Devuelve un objeto Range que representa la región actual. La región actual es un rango delimitado por cualquier combinación de filas en blanco y columnas en blanco.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Obtiene un objeto Range que representa la columna completa (o columnas) que contiene el rango especificado.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Obtiene un objeto Range que representa la fila completa (o filas) que contiene el rango especificado.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Obtiene el índice de la primera columna del rango.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Obtiene el índice de la primera fila del rango.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtiene el ancho de un rango en puntos.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Obtiene todos los hipervínculos en el rango.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del rango.

**Remarks**

Se admite rango con nombre. Por ejemplo,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Obtiene el [Range](../../com.aspose.cells/range) por desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | int | Desplazamiento de columna en este rango, basado en cero. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Obtiene a qué se refiere el rango.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtiene la cantidad de filas en el rango.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Establece u obtiene la altura de las filas en este rango

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor del rango.

**Remarks**

Si el rango contiene varias celdas, el objeto devuelto/aplicado debe ser Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtiene el ancho de un rango en puntos.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene el objeto [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) que contiene este rango.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


Devuelve un objeto [Range](../../com.aspose.cells/range) que representa la intersección rectangular de dos rangos.

**Remarks**

Si los dos rangos no se intersectan, devuelve null.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango de intersección. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indica si el rango contiene valores.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Indica si el rango se intersecta.

**Remarks**

Si los dos rangos no están en la misma hoja de cálculo, devuelve false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango. |

**Returns:**
boolean - Indica si el rango se intersecta.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de celdas en este Range.

**Remarks**

Al recorrer los elementos mediante el Enumerator devuelto, la colección de celdas no debe modificarse (por ejemplo, operaciones que provoquen la creación de una nueva Cell/Row o la eliminación de una Cell/Row existente). De lo contrario, el enumerador podría no ser capaz de recorrer todas las celdas correctamente (algunos elementos podrían recorrerse repetidamente o omitirse).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - El enumerador de celdas
### merge() {#merge--}
```
public void merge()
```


Combina un rango de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda del rango.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Mueve el rango actual al rango de destino.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destRow | int | La fila de inicio del rango de destino. |
| destColumn | int | La columna de inicio del rango de destino. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Introduce un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | boolean | True: establece el formato numérico en el estilo de la celda al convertir a otro tipo de datos |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Establece u obtiene el ancho de columna de este rango

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Establece los bordes internos del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Dentro del tipo de borde, solo puede ser [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) y [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). El estilo de borde. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | El color del borde. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre del rango.

**Remarks**

Se admite rango con nombre. Por ejemplo,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Establece el borde de contorno alrededor de un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Borde. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de borde. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Color del borde. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Establece el borde de contorno alrededor de un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Borde. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de borde. |
| borderColor | [Color](../../com.aspose.cells/color) | Color del borde. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de borde. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Color del borde. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Establece los bordes de contorno alrededor de un rango de celdas con el mismo estilo y color de borde.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilo de borde. |
| borderColor | [Color](../../com.aspose.cells/color) | Color del borde. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Establece los bordes externos alrededor de un rango de celdas.

**Remarks**

Ambas longitudes de borderStyles y borderStyles deben ser 4. El orden de borderStyles y borderStyles debe ser top,bottom,left,right

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Estilos de borde. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Colores del borde. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Establece u obtiene la altura de las filas en este rango

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Establece el estilo del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El objeto Style. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Aplica el estilo de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El estilo de la celda. |
| explicitFlag | boolean | Verdadero, solo sobrescribiendo el formato que está establecido explícitamente. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece el valor del rango.

**Remarks**

Si el rango contiene varias celdas, el objeto devuelto/aplicado debe ser Object[][].

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Convierte el rango a HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Opciones para convertir el rango a html. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Convierte el rango a imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Las opciones para convertir este rango a imagen |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Convierte el rango a valor JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Las opciones de conversión |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Range actual.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Transpone (rota) datos de filas a columnas o viceversa.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Descombina celdas combinadas de este rango.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Devuelve la unión de dos rangos.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Range.UnionRanges(). Este método será eliminado 12 meses después desde noviembre de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango |

**Returns:**
java.util.ArrayList - La unión de dos rangos.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Devuelve el resultado de la unión de dos rangos.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Range.UnionRanges(). Este método será eliminado 12 meses después desde mayo de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | El rango |

**Returns:**
com.aspose.cells.Range[] - La unión de dos rangos.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Devuelve el resultado de la unión de dos rangos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | El rango |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

