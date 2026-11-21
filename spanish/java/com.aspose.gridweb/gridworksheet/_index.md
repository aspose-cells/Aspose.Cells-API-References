---
title: "GridWorksheet"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una sola hoja de cálculo."
type: docs
url: /es/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Encapsula el objeto que representa una sola hoja de cálculo.
## Métodos

| Método | Descripción |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Establece el rango al que se aplica el AutoFilter especificado. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Agregar filtro personalizado para la fila especificada. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajusta automáticamente el ancho de la columna. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Ajusta automáticamente el ancho de la columna. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Ajusta automáticamente la altura de la fila. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Ajusta automáticamente la altura de la fila. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Ajusta automáticamente la altura de la fila en un rango rectangular. |
| [autoFitRows()](#autoFitRows--) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Ajusta automáticamente la altura de la fila en un rango. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcula una fórmula. |
| [clearComments()](#clearComments--) | Elimina todos los comentarios en la hoja de cálculo del diseñador. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Copia el contenido y los formatos de otra hoja de cálculo. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Crea un subtotal en la hoja. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crea un subtotal en la hoja. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de invocar filterString. La cadena de criterios del filtro. Nota: usamos la coma -> "," como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,"123,456") significa que la columna 10 debe contener 123 o 456, filterString(10,"123") significa que la columna 10 debe contener 123. El índice de columna se separa con comas, p. ej. 123,456,789 o abc. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [getActiveCell()](#getActiveCell--) | Obtiene la celda activa en la hoja de cálculo. |
| [getBackgroundImage()](#getBackgroundImage--) | Obtiene la imagen de fondo de la hoja de cálculo. |
| [getCells()](#getCells--) | Obtiene la colección de [GridCell](../../com.aspose.gridweb/gridcell). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Representa el nombre de código de la hoja de cálculo. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Obtiene el título de la columna. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Obtiene el texto de información sobre herramientas del encabezado de columna. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Obtiene si una columna es de solo lectura. |
| [getComments()](#getComments--) | Obtiene la colección de [GridComment](../../com.aspose.gridweb/gridcomment). |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. |
| [getDisplayZeros()](#getDisplayZeros--) | Verdadero si se muestran valores cero. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Representa el índice de la primera columna visible. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Representa el índice de la primera fila visible. |
| [getFreezedPanes()](#getFreezedPanes--) | Obtiene los paneles congelados. |
| [getGridActiveCell()](#getGridActiveCell--) | Obtiene la celda activa en la hoja de cálculo. |
| [getHyperlinks()](#getHyperlinks--) | Obtiene la colección de [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection). |
| [getIndex()](#getIndex--) | Obtiene el índice de la hoja en la colección de hojas de cálculo. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Obtiene si la celda es de solo lectura. Este es un atributo extendido de GridWeb ,no se conservará en el archivo Excel real. |
| [getName()](#getName--) | Obtiene el nombre de la hoja de cálculo. |
| [getOutlineShown()](#getOutlineShown--) | Indica si se muestra el contorno. |
| [getPictures()](#getPictures--) | Obtiene una colección de [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--). |
| [getPivotTables()](#getPivotTables--) | Obtiene las tablas dinámicas en la hoja de cálculo. |
| [getRowCaption(int row)](#getRowCaption-int-) | Obtiene el título de la fila. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Obtiene el texto de información sobre herramientas del encabezado de fila. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Obtiene si una fila es de solo lectura. |
| [getSelected()](#getSelected--) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro. |
| [getShapes()](#getShapes--) | Obtiene una colección de [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--). |
| [getStandardHeight()](#getStandardHeight--) | Obtiene la altura predeterminada de la fila en esta hoja, en unidades de puntos. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Obtiene la altura predeterminada de la fila en esta hoja, en unidades de píxeles. |
| [getTabColor()](#getTabColor--) | Representa el color de la pestaña de la hoja de cálculo. |
| [getUniqueID()](#getUniqueID--) | Obtiene el UniqueID en el Control |
| [getValidations()](#getValidations--) | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| [getVisible()](#getVisible--) | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto [GridWorkbook](../../com.aspose.gridweb/gridworkbook) de la colección de hojas de cálculo. |
| [getZoom()](#getZoom--) | Representa el factor de escala en porcentaje. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Agrupa filas. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Obtiene un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true. |
| [isProtected()](#isProtected--) | Indica si la hoja de cálculo está protegida. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema. |
| [moveTo(int index)](#moveTo-int-) | Mueve la hoja a otra ubicación en la hoja de cálculo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Actualiza los filtros automáticos para ocultar o mostrar las filas. |
| [removeAutoFilter()](#removeAutoFilter--) | Elimina el filtro automático de la hoja de cálculo. |
| [removeSubtotal()](#removeSubtotal--) | Elimina el subtotal creado por el método CreateSubtotal en la hoja. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | El desplazamiento entero del campo al que desea aplicar, basado en la primera columna de filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Establece la celda activa en la hoja de cálculo. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Hace que todas las celdas sean editables. Este es un atributo extendido. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Hace que todas las celdas sean de solo lectura. Este es un atributo extendido; tenga en cuenta que este atributo no se puede mantener en la celda real; si desea mantener la protección, por favor use setProtect. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Establece la imagen de fondo de la hoja de cálculo. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Establece el título para la columna. Tenga en cuenta que este es un atributo de extensión y no se puede conservar en el archivo de Excel. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Establece el texto de información sobre herramientas del encabezado de columna. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Establece una columna como de solo lectura para que el usuario no pueda eliminarla del lado del cliente. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Verdadero si se muestran valores cero. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga que todas las celdas sean de solo lectura llamando al método SetAllCellsReadonly. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Representa el índice de la primera columna visible. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Representa el índice de la primera fila visible. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Establece la celda activa en la hoja de cálculo. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Establece un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Establece si la celda es de solo lectura. Este es un atributo extendido de GridWeb; no se conservará en el archivo de Excel real. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la hoja de cálculo. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indica si se muestra el contorno. |
| [setProtect()](#setProtect--) | Protege la hoja de cálculo. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga que todas las celdas sean editables llamando al método SetAllCellsEditable. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Establece el título para la fila. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Establece el texto de información sobre herramientas del encabezado de fila. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Establece una fila como de solo lectura para que el usuario no pueda eliminarla del lado del cliente. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de puntos. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Establece la altura predeterminada de la fila en esta hoja de cálculo, en unidades de píxeles. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Representa el color de la pestaña de la hoja de cálculo. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |
| [setZoom(int value)](#setZoom-int-) | Representa el factor de escala en porcentaje. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Descongela los paneles en la hoja de cálculo. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Desagrupa filas. |
| [unProtect()](#unProtect--) | Desprotege la hoja de cálculo. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Establece el rango al que se aplica el AutoFilter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Agregar filtro personalizado para la fila especificada.

**Remarks**

La cadena de criterios de filtro. Tenga en cuenta que usamos , y ; como caracteres de separación, por lo que el valor de la celda no debe contener esos caracteres. A continuación se presentan ejemplos de la cadena de criterios //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int |  |
| criterio | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Ajusta automáticamente el ancho de la columna.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Ajusta automáticamente el ancho de la columna.

**Remarks**

Este método ajusta automáticamente una fila según el contenido en un rango de celdas dentro de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | Índice de columna. |
| firstRow | int | Índice de la primera fila. |
| lastRow | int | Índice de la última fila. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Ajusta automáticamente la altura de la fila.

**Remarks**

AutoFitRow es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Ajusta automáticamente la altura de la fila.

**Remarks**

Este método ajusta automáticamente una fila según el contenido en un rango de celdas dentro de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | Índice de fila. |
| firstColumn | int | Índice de la primera columna. |
| lastColumn | int | Último índice de columna. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Ajusta automáticamente la altura de la fila en un rango rectangular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Ajusta automáticamente todas las filas en esta hoja de cálculo.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Ajusta automáticamente todas las filas en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| onlyAuto | boolean | True, solo ajusta automáticamente la altura de la fila cuando la altura de la fila no está personalizada. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Ajusta automáticamente la altura de la fila en un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcula una fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


Elimina todos los comentarios en la hoja de cálculo del diseñador.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Copia el contenido y los formatos de otra hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Hoja de origen. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Crea un subtotal en la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnNameRowIndex | int | El índice de fila de la fila de nombre de columna. |
| dataRows | int | El número de filas de datos. |
| groupByColumnIndex | int | El índice de columna de la columna que se agrupará. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). El tipo de función de subtotal. |
| subtotalColumnIndexList | int[] | Los índices de columna que se subtotalearán. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Crea un subtotal en la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnNameRowIndex | int | El índice de fila de la fila de nombre de columna. |
| dataRows | int | El número de filas de datos. |
| groupByColumnIndex | int | El índice de columna de la columna que se agrupará. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). El tipo de función de subtotal. |
| subtotalColumnIndexList | int[] | Los índices de columna que se subtotalearán. |
| functionLabel | java.lang.String | La etiqueta de la función de subtotal. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El estilo de la línea de total general. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | El estilo de la línea de subtotal. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). El tipo numérico de las celdas de resultado del subtotal. |
| customString | java.lang.String | La cadena de formato personalizada de las celdas de resultado del subtotal. Puede ser nula. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de invocar filterString. La cadena de criterios del filtro. Nota: usamos la coma -> "," como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,"123,456") significa que la columna 10 debe contener 123 o 456, filterString(10,"123") significa que la columna 10 debe contener 123. El índice de columna se separa con comas, p. ej. 123,456,789 o abc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int |  |
| criterios | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Congela paneles en la celda especificada de la hoja de cálculo.

**Remarks**

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

Los dos primeros parámetros especifican la posición congelada y los dos últimos parámetros especifican el área congelada en el panel superior izquierdo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| columna | int | Índice de columna. |
| freezedRows | int | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | int | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Congela paneles en la celda especificada de la hoja de cálculo.

**Remarks**

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de celda. |
| freezedRows | int | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | int | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Obtiene la celda activa en la hoja de cálculo.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Obtiene la imagen de fondo de la hoja de cálculo.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Obtiene la colección de [GridCell](../../com.aspose.gridweb/gridcell).

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Representa el nombre de código de la hoja de cálculo.

**Remarks**

No puedes cambiar el nombre del código mientras el archivo de plantilla contiene VBA/macros.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Obtiene el título de la columna. Si el título no está establecido, devuelve una cadena vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |

**Returns:**
java.lang.String - El título de la columna. Si el título no está establecido, devuelve una cadena vacía.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Obtiene el texto de información sobre herramientas del encabezado de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| colIndex | int | El índice de la columna. |

**Returns:**
java.lang.String - El texto de información sobre herramientas.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Obtiene si una columna es de solo lectura. Este es un método extendido de GridWeb específicamente, no se mantendrá ni tendrá efecto en el archivo Excel real.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna. |

**Returns:**
boolean - Si es de solo lectura devuelve true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Obtiene la colección de [GridComment](../../com.aspose.gridweb/gridcomment).

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Verdadero si se muestran valores cero.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Representa el índice de la primera columna visible.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Representa el índice de la primera fila visible.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Obtiene los paneles congelados.

**Returns:**
int[] - Devolver null significa que la hoja de cálculo no está congelada 0:índice de fila;1:columna;2:filas congeladas;3:filas congeladas
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Obtiene la celda activa en la hoja de cálculo.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Obtiene la colección de [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection).

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de la hoja en la colección de hojas de cálculo.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Obtiene si la celda es de solo lectura. Este es un atributo extendido de GridWeb ,no se conservará en el archivo Excel real.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la hoja de cálculo.

**Remarks**

La longitud máxima del nombre de la hoja es 31. Y no puede asignar el mismo nombre (sin distinción de mayúsculas) a dos hojas de cálculo. Por ejemplo, no puede establecer "SheetName1" en la primera hoja y "SHEETNAME1" en la segunda hoja.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Indica si se muestra el contorno.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Obtiene una colección de [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--).

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Obtiene las tablas dinámicas en la hoja de cálculo.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Obtiene el título de la fila. Si el título no está establecido, devuelve una cadena vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |

**Returns:**
java.lang.String - El título de la fila. Si el título no está establecido, devuelve una cadena vacía.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Obtiene el texto de información sobre herramientas del encabezado de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de la fila. |

**Returns:**
java.lang.String - El texto de información sobre herramientas.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Obtiene si una fila es de solo lectura. Este es un método extendido de GridWeb específicamente, no se mantendrá ni tendrá efecto en el archivo Excel real

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila. |

**Returns:**
boolean - Si es de solo lectura devuelve true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Indica si esta hoja de cálculo está seleccionada cuando se abre el libro.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Obtiene una colección de [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--).

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
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
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Representa el color de la pestaña de la hoja de cálculo.

**Remarks**

Esta característica solo es compatible con ExcelXP (Excel2002) y versiones posteriores. Si guarda el archivo en formato Excel97 o Excel2000, se omitirá.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtiene el UniqueID en el Control

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Obtiene el objeto [GridWorkbook](../../com.aspose.gridweb/gridworkbook) de la colección de hojas de cálculo.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Returns:**
int
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Agrupa filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a agrupar. |
| lastIndex | int | El índice de la última fila a agrupar. |
| isHidden | boolean | Especifica si las filas agrupadas están ocultas. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Obtiene un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica si la hoja de cálculo está protegida.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Mueve la hoja a otra ubicación en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice de la hoja de destino. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Actualiza los filtros automáticos para ocultar o mostrar las filas.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Elimina el filtro automático de la hoja de cálculo.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Elimina el subtotal creado por el método CreateSubtotal en la hoja.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


El desplazamiento entero del campo al que desea aplicar, basado en la primera columna de filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Establece la celda activa en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Hace que todas las celdas sean editables. Este es un atributo extendido.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Hace que todas las celdas sean de solo lectura. Este es un atributo extendido; tenga en cuenta que este atributo no se puede mantener en la celda real; si desea mantener la protección, por favor use setProtect.

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Establece la imagen de fondo de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Establece el título para la columna. Tenga en cuenta que este es un atributo de extensión y no se puede conservar en el archivo de Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | int | Índice de columna. |
| leyenda | java.lang.String | La leyenda de la columna. Pase null o una cadena vacía si desea cancelar la leyenda. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Establece el texto de información sobre herramientas del encabezado de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| colIndex | int | El índice de la columna. |
| texto emergente | java.lang.String | El texto del tooltip. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Establece una columna como solo lectura para que el usuario no pueda eliminarla del lado del cliente. Este es un método extendido de GridWeb específicamente, no se mantendrá ni tendrá efecto en el archivo Excel real

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna. |
| isReadonly | boolean | verdadero o falso. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Verdadero si se muestran valores cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga todas las celdas de solo lectura llamando al método SetAllCellsReadonly. Luego llame a este método para especificar el rango de celdas que debe ser editable

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial del rango. |
| startColumn | int | La columna inicial del rango. |
| filas | int | El número de filas. |
| columnas | int | El número de columnas. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Representa el índice de la primera columna visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Representa el índice de la primera fila visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Establece la celda activa en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Establece un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Establece si la celda es de solo lectura. Este es un atributo extendido de GridWeb; no se conservará en el archivo de Excel real.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int |  |
| col | int |  |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la hoja de cálculo.

**Remarks**

La longitud máxima del nombre de la hoja es 31. Y no puede asignar el mismo nombre (sin distinción de mayúsculas) a dos hojas de cálculo. Por ejemplo, no puede establecer "SheetName1" en la primera hoja y "SHEETNAME1" en la segunda hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Indica si se muestra el contorno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Protege la hoja de cálculo.

**Remarks**

Este método protege la hoja de cálculo sin contraseña. Puede proteger la hoja de cálculo en todas las versiones del archivo de Excel.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga todas las celdas editables llamando al método SetAllCellsEditable. Luego llame a este método para especificar el rango de celdas que debe ser de solo lectura

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial del rango. |
| startColumn | int | La columna inicial del rango. |
| filas | int | El número de filas. |
| columnas | int | El número de columnas. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Establece el título para la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| leyenda | java.lang.String | La leyenda de la fila. Pase null o una cadena vacía si desea cancelar la leyenda. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Establece el texto de información sobre herramientas del encabezado de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | El índice de la fila. |
| texto emergente | java.lang.String | El texto del tooltip. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Establece una fila como solo lectura para que el usuario no pueda eliminarla del lado del cliente. Este es un método extendido de GridWeb específicamente, no se mantendrá ni tendrá efecto en el archivo Excel real

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | índice de fila. |
| isReadonly | boolean | verdadero o falso. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica si esta hoja de cálculo está seleccionada cuando se abre el libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Representa el color de la pestaña de la hoja de cálculo.

**Remarks**

Esta característica solo es compatible con ExcelXP (Excel2002) y versiones posteriores. Si guarda el archivo en formato Excel97 o Excel2000, se omitirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Descongela los paneles en la hoja de cálculo.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Desagrupa filas.

**Remarks**

Solo elimina la información del grupo externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | int | El índice de la primera fila a desagrupar. |
| lastIndex | int | El índice de la última fila a desagrupar. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Desprotege la hoja de cálculo.

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

