---
title: "GridCells"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Encapsula una colección de objetos [GridCell](../../com.aspose.gridweb/gridcell).
## Métodos

| Método | Descripción |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Obtiene los índices de fila y columna de la celda según su nombre |
| [checkCell(int row, int column)](#checkCell-int-int-) | Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) o null en el índice de fila y columna de celda especificados. |
| [checkColumn(int col)](#checkColumn-int-) | Obtiene el elemento [GridColumn](../../com.aspose.gridweb/gridcolumn) o null en el índice de columna especificado. |
| [checkRow(int i)](#checkRow-int-) | Obtiene el elemento [GridRow](../../com.aspose.gridweb/gridrow) o null en el índice de fila de celda especificado. |
| [clear()](#clear--) | Borra todas las celdas de la colección. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Borra el contenido de un rango. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Borra el contenido de un rango. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Borra el formato de un rango. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Borra el formato de un rango. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Borra el contenido y el formato de un rango. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Borra el contenido y el formato de un rango. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Obtiene el nombre de la columna según el índice de columna. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Obtiene el índice de columna según el nombre de la columna. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Copia los datos y formatos de una columna completa. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Copia los datos y formatos de una columna completa. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Copia los datos y formatos de una fila completa. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Copia los datos y formatos de varias filas completas. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Elimina todas las columnas en blanco que no contienen datos. |
| [deleteBlankRows()](#deleteBlankRows--) | Elimina todas las filas en blanco que no contienen datos. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Elimina una columna. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Elimina una columna. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Elimina varias columnas. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Elimina una fila. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Elimina varias filas. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Elimina varias filas en la hoja de cálculo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporta los datos de la colección [GridCells](../../com.aspose.gridweb/gridcells) a un objeto de matriz bidimensional. |
| [get(int row, int column)](#get-int-int-) | Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el índice de fila y columna de celda especificados. |
| [get(String cellName)](#get-java.lang.String-) | Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el nombre de celda especificado. |
| [getCell(int row, int column)](#getCell-int-int-) | Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el índice de fila y columna de celda especificados. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Obtiene el ancho de la columna especificada |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Obtiene el ancho de la columna especificada, en unidades de pulgadas. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Obtiene el ancho de la columna especificada, en unidades de píxeles. |
| [getColumns()](#getColumns--) | Obtiene la colección de objetos [GridColumn](../../com.aspose.gridweb/gridcolumn) que representan las columnas individuales en esta hoja de cálculo. |
| [getCount()](#getCount--) | Obtiene el número de celdas. |
| [getFirstCell()](#getFirstCell--) | Obtiene la primera celda en esta hoja de cálculo. |
| [getLastCell()](#getLastCell--) | Obtiene la última celda en esta hoja de cálculo. |
| [getMaxColumn()](#getMaxColumn--) | Índice máximo de columna de la celda que contiene datos o estilo. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Índice máximo de columna de la celda que contiene datos. |
| [getMaxDataRow()](#getMaxDataRow--) | Índice máximo de fila de la celda que contiene datos. |
| [getMaxRow()](#getMaxRow--) | Índice máximo de fila de la celda que contiene datos o estilo. |
| [getMergedCells()](#getMergedCells--) | Obtiene la colección de celdas combinadas. |
| [getMinColumn()](#getMinColumn--) | Índice de columna mínimo de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [getMinDataColumn()](#getMinDataColumn--) | Índice de columna mínimo de la celda que contiene datos. |
| [getMinDataRow()](#getMinDataRow--) | Índice de fila mínimo de la celda que contiene datos. |
| [getMinRow()](#getMinRow--) | Índice de fila mínimo de la celda que contiene datos o estilo. |
| [getRow(int i)](#getRow-int-) | Obtiene el elemento [GridRow](../../com.aspose.gridweb/gridrow) en el índice de fila de celda especificado. |
| [getRowEnumerator()](#getRowEnumerator--) | Obtiene el enumerador de filas |
| [getRowHeight(int row)](#getRowHeight-int-) | Obtiene la altura de una fila especificada. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Obtiene la altura de una fila especificada en unidades de píxeles. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Obtiene el nivel de contorno de la fila. |
| [getRows()](#getRows--) | Obtiene la colección de objetos [GridRow](../../com.aspose.gridweb/gridrow) que representan las filas individuales en esta hoja de cálculo. |
| [getStandardHeight()](#getStandardHeight--) | Obtiene la altura predeterminada de la fila en esta hoja, en unidades de puntos. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtiene la altura predeterminada de la fila en esta hoja, en unidades de píxeles. |
| [getStandardWidth()](#getStandardWidth--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Obtenga el ancho en diferentes tipos de vista. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Agrupa columnas. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Agrupa columnas. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Agrupa filas. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Oculta una columna. |
| [hideRow(int row)](#hideRow-int-) | Oculta una fila. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserta una nueva columna en la hoja de cálculo. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserta una nueva columna en la hoja de cálculo. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserta varias columnas en la hoja de cálculo. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserta varias columnas en la hoja de cálculo. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserta una nueva fila en la hoja de cálculo. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserta varias filas en la hoja de cálculo. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserta varias filas en la hoja de cálculo. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Comprueba si la columna dada está vacía (no contiene datos). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Comprueba si una columna en el índice dado está oculta. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Comprueba si una fila en el índice dado está oculta. |
| [iterator()](#iterator--) | Obtiene el enumerador de filas |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Fusiona un rango especificado de celdas en una sola celda. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Mueve el rango. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Elimina los valores duplicados en el rango. |
| [removeFormulas()](#removeFormulas--) | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Establece bordes para un rango de celdas. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Establece el ancho de la columna especificada. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Establece el ancho de columna en unidades de pulgadas. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Establece el ancho de columna en unidades de píxeles. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Establece la altura de la fila especificada. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Establece la altura de la fila en unidades de pulgadas. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Establece la altura de la fila en unidades de píxeles. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Establece el nivel de contorno de la fila. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de puntos. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de píxeles. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de pulgadas. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de píxeles. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo a un rango especificado de celdas. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Establece el estilo a un rango especificado de celdas. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Descombina un rango especificado de celdas combinadas. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Desagrupa columnas. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Desagrupa filas. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Desoculta una columna |
| [unhideRow(int row)](#unhideRow-int-) | Desoculta una fila. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Obtiene el nombre de la celda según sus índices de fila y columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |

**Returns:**
java.lang.String - Nombre de la celda.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Obtiene los índices de fila y columna de la celda según su nombre

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de la celda. |
| fila | int | Índice de fila de salida |
| columna | int | Índice de columna de salida |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) o null en el índice de fila y columna de celda especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |
| columna | int | Índice de columna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Obtiene el elemento [GridColumn](../../com.aspose.gridweb/gridcolumn) o null en el índice de columna especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| col | int | El índice de columna. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Obtiene el elemento [GridRow](../../com.aspose.gridweb/gridrow) o null en el índice de fila de celda especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| i | int | Índice de fila |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Borra todas las celdas de la colección.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Borra el contenido de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Rango a borrar. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el contenido de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Borra el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Rango a borrar. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Borra el contenido y el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Rango a borrar. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Borra el contenido y el formato de un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Obtiene el nombre de la columna según el índice de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

**Returns:**
java.lang.String - Nombre de la columna.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Obtiene el índice de columna según el nombre de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnName | java.lang.String | Nombre de columna. |

**Returns:**
int - Índice de columna.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copia los datos y formatos de una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copia los datos y formatos de una columna completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | int | Índice de columna de origen. |
| destinationColumnIndex | int | Índice de columna de destino. |
| columnNumber | int | El número de columna copiada. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copia los datos y formatos de una fila completa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copia los datos y formatos de varias filas completas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | int | Índice de fila de origen. |
| destinationRowIndex | int | Índice de fila de destino. |
| rowNumber | int | El número de fila copiada. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Elimina todas las columnas en blanco que no contienen datos.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Elimina todas las filas en blanco que no contienen datos.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Elimina una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Elimina una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| updateReference | boolean | Indica si actualizar referencias en otras hojas de cálculo. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Elimina varias columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | Número de columnas a eliminar. |
| updateReference | boolean | Indica si actualizar referencias en otras hojas de cálculo. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| startColumn | int | Índice de columna inicial. |
| endRow | int | Índice de fila final. |
| endColumn | int | Índice de columna final. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opción de desplazamiento de celdas. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Elimina una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Elimina varias filas.

**Remarks**

Si el rango eliminado contiene la parte superior (no completa) de la tabla (ListObject), el rango no se puede eliminar y no se hará nada. Funciona como MS Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de la primera fila a eliminar. |
| totalRows | int | Número de filas a eliminar. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Elimina varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a eliminar. |
| updateReference | boolean | Indica si actualizar referencias en otras hojas de cálculo. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporta los datos de la colección [GridCells](../../com.aspose.gridweb/gridcells) a un objeto de matriz bidimensional.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | El número de fila de la primera celda a exportar. |
| firstColumn | int | El número de columna de la primera celda a exportar |
| totalRows | int | Número de filas a exportar |
| totalColumns | int | Número de columnas a exportar |

**Returns:**
java.lang.Object[][] - Objeto de matriz de valores de celda exportados.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el índice de fila y columna de celda especificados.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el nombre de celda especificado.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de la celda, incluyendo su letra de columna y número de fila, por ejemplo A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Obtiene el elemento [GridCell](../../com.aspose.gridweb/gridcell) en el índice de fila y columna de celda especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |
| columna | int | Índice de columna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Obtiene el ancho de la columna especificada

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
double - Ancho de columna
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Obtiene el ancho de la columna especificada, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
double - Ancho de columna
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Obtiene el ancho de la columna especificada, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna |

**Returns:**
int - Ancho de la columna en vista normal.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Obtiene la colección de objetos [GridColumn](../../com.aspose.gridweb/gridcolumn) que representan las columnas individuales en esta hoja de cálculo.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de celdas.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Obtiene la primera celda en esta hoja de cálculo.

**Remarks**

Devuelve null si no hay datos en la hoja de cálculo.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Obtiene la última celda en esta hoja de cálculo.

**Remarks**

Devuelve null si no hay datos en la hoja de cálculo.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Índice máximo de columna de la celda que contiene datos o estilo.

**Remarks**

Devuelve -1 si no hay celda.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Índice máximo de columna de la celda que contiene datos.

**Remarks**

\-1 será devuelto si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar todas las celdas en una hoja de cálculo, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Índice máximo de fila de la celda que contiene datos.

**Remarks**

Devuelve -1 si no hay ninguna celda que contenga datos.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Índice máximo de fila de la celda que contiene datos o estilo.

**Remarks**

Devuelve -1 si no hay ninguna celda que contenga datos o estilo en la hoja de cálculo.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Obtiene la colección de celdas combinadas.

**Remarks**

En esta colección, cada elemento es una estructura [GridCellArea](../../com.aspose.gridweb/gridcellarea) que representa un área de celdas combinadas.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Índice de columna mínimo de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Índice de columna mínimo de la celda que contiene datos.

**Remarks**

\-1 será devuelto si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar todas las celdas en una hoja de cálculo, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Índice de fila mínimo de la celda que contiene datos.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Índice de fila mínimo de la celda que contiene datos o estilo.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Obtiene el elemento [GridRow](../../com.aspose.gridweb/gridrow) en el índice de fila de celda especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| i | int | Índice de fila |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Obtiene el enumerador de filas

**Returns:**
java.util.Iterator - El enumerador de filas.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Obtiene la altura de una fila especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
double - Altura de la fila
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Obtiene la altura de una fila especificada en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
double - Altura de la fila
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Obtiene la altura de una fila especificada en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila |

**Returns:**
int - Altura de la fila
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Obtiene el nivel de contorno de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila. |

**Returns:**
int - el nivel de esquema.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Obtiene la colección de objetos [GridRow](../../com.aspose.gridweb/gridrow) que representan las filas individuales en esta hoja de cálculo.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Obtiene la altura predeterminada de la fila en esta hoja, en unidades de puntos.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Obtiene la altura predeterminada de la fila en esta hoja, en unidades de píxeles.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Obtiene el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Obtenga el ancho en diferentes tipos de vista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | El índice de columna. |

**Returns:**
int - el ancho de la columna en unidades de píxeles
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Agrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a agrupar. |
| lastIndex | int | El índice de la última columna a agrupar. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Agrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a agrupar. |
| lastIndex | int | El índice de la última columna a agrupar. |
| isHidden | boolean | Especifica si las columnas agrupadas están ocultas. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Oculta una columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Oculta una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Inserta una nueva columna en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Inserta una nueva columna en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Inserta varias columnas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | El número de columnas. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Inserta varias columnas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| totalColumns | int | El número de columnas. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Desplazar área. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opción de desplazamiento de celdas. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Desplazar área. |
| shiftNumber | int | Número de filas o columnas a insertar. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opción de desplazamiento de celdas. |
| updateReference | boolean | Indica si actualizar referencias en otras hojas de cálculo. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Inserta una nueva fila en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Inserta varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a insertar. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Inserta varias filas en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| totalRows | int | Número de filas a insertar. |
| updateReference | boolean | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Comprueba si la columna dada está vacía (no contiene datos).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | el índice de columna |

**Returns:**
booleano - verdadero si la columna dada no contiene datos
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Comprueba si una columna en el índice dado está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna |

**Returns:**
booleano - verdadero si la columna está oculta.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Comprueba si una fila en el índice dado está oculta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila |

**Returns:**
booleano - verdadero si la fila está oculta
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene el enumerador de filas

**Returns:**
java.util.Iterator - El enumerador de filas
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Fusiona un rango especificado de celdas en una sola celda.

**Remarks**

Referencia la celda combinada mediante la dirección de la celda superior izquierda del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Mueve el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El rango que debe moverse. |
| destRow | int | La fila de destino. |
| destColumn | int | La columna de destino. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Elimina los valores duplicados en el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial |
| endRow | int | El índice de fila final. |
| endColumn | int | El índice de columna final. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Elimina todas las fórmulas y las reemplaza con el valor de la fórmula.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Establece bordes para un rango de celdas.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | El número de fila inicial del rango (basado en cero). |
| firstColumn | int | El número de columna inicial del rango (basado en cero). |
| rowNumber | int | El número de filas. |
| columnNumber | int | El número de columnas. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). La posición del borde. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | El estilo del borde. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Establece el ancho de la columna especificada.

**Remarks**

Para ocultar una columna, establece el ancho de la columna a cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| ancho | double | Ancho de la columna. El ancho de la columna debe estar entre 0 y 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Establece el ancho de columna en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| pulgadas | double | Número de pulgadas. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Establece el ancho de columna en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| píxel | int | Número de píxeles. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Establece la altura de la fila especificada.

**Remarks**

Para ocultar una fila, establece la altura de la fila a cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| altura | double | Altura de fila. En unidades de punto. Debe estar entre 0 y 409.5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Establece la altura de la fila en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| pulgadas | double | Número de pulgadas. Debe estar entre 0 y 409.5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Establece la altura de la fila en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| píxeles | int | Número de píxeles. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Establece el nivel de contorno de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila. |
| outlineLevel | int | nivel de esquema. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de puntos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Establece el ancho predeterminado de la columna en la hoja de cálculo, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Establece el estilo a un rango especificado de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| rowNumber | int | Número de filas (basado en uno) |
| columnNumber | int | Número de columnas (basado en uno) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El objeto de estilo a establecer |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Establece el estilo a un rango especificado de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellRange | java.lang.String | El rango de nombres de celdas, como "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El objeto de estilo a establecer |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo según el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo según el índice de fila especificado.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | El número de fila de la primera celda a ordenar. |
| startColumn | int | El número de columna de la primera celda a ordenar. |
| filas | int | Número de filas a importar. |
| columnas | int | Número de columnas a importar. |
| índice | int | El índice de columna que especifica la columna de ordenación. Si la orientación es de arriba a abajo, representa el índice de columna que especifica la columna de ordenación. Si la orientación es de izquierda a derecha, representa el índice de fila que especifica la fila de ordenación. |
| isAsending | boolean | si el orden de clasificación es ascendente . |
| isCaseSensitive | boolean | si la ordenación es sensible a mayúsculas y minúsculas . |
| islefttoright | boolean | si la orientación de la ordenación es de izquierda a derecha |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo según el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo según el índice de fila especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | El número de fila de la primera celda a ordenar. |
| startColumn | int | El número de columna de la primera celda a ordenar. |
| filas | int | Número de filas a importar. |
| columnas | int | Número de columnas a importar. |
| índices | int[] | La matriz de índices de columna que especifica la columna de ordenación. si la Orientation es de arriba a abajo, representa el índice de columna que especifica la columna de ordenación. si la Orientation es de izquierda a derecha, representa el índice de fila que especifica la fila de ordenación. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). el arreglo de orden de clasificación . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). orientación de ordenación |
| isCaseSensitive | boolean | si la ordenación es sensible a mayúsculas y minúsculas . |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Descombina un rango especificado de celdas combinadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila de este rango (basado en cero) |
| firstColumn | int | Primera columna de este rango (basado en cero) |
| totalRows | int | Número de filas (basado en uno) |
| totalColumns | int | Número de columnas (basado en uno) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Desagrupa columnas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera columna a desagrupar. |
| lastIndex | int | El índice de la última columna a desagrupar. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Desagrupa filas.

**Remarks**

Solo elimina la información del grupo externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a desagrupar. |
| lastIndex | int | El índice de la última fila a desagrupar. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Desoculta una columna

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| ancho | double | Ancho de columna..El ancho de columna debe estar entre 0 y 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Desoculta una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

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

