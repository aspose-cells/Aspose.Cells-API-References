---
title: "ExportTableOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las opciones de exportación de tabla."
type: docs
url: /es/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Representa todas las opciones de exportación de tabla.

**Remarks**

Si existen requisitos especiales sobre la exportación, como ignorar valores de error, el usuario puede extender esta clase para sobrescribir las APIs correspondientes y lograr el objetivo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Este valor indica si se permiten DBNulls en esta tabla. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells establecerá el tipo de DataColumn según el tipo de valor de la primera fila para mejorar el rendimiento. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exporta el valor de cadena html de las celdas al DataTable. |
| [getExportAsString()](#getExportAsString--) | Exporta el valor de cadena de las celdas al DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtiene la estrategia de formato al exportar el valor como cadena. |
| [getIndexes()](#getIndexes--) | Los índices de columnas/filas que deben exportarse. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Solo exporta celdas visibles. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Solo exporta columnas visibles. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Solo exporta filas visibles. |
| [getRenameStrategy()](#getRenameStrategy--) | Estrategia para nombres duplicados de columnas. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indica si se omite el valor inválido para la columna. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | Verdadero si una fila en el archivo Workbook representa una fila en DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Preprocesa el valor de la celda actual para exportarla. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Este valor indica si se permiten DBNulls en esta tabla. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells establecerá el tipo de DataColumn según el tipo de valor de la primera fila para mejorar el rendimiento. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Exporta el valor de cadena html de las celdas al DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exporta el valor de cadena de las celdas al DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Establece la estrategia de formato al exportar el valor como cadena. |
| [setIndexes(int[] value)](#setIndexes-int---) | Los índices de columnas/filas que deben exportarse. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Solo exporta celdas visibles. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Solo exporta columnas visibles. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Solo exporta filas visibles. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Estrategia para nombres duplicados de columnas. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Indica si se omite el valor inválido para la columna. |
| [setVertical(boolean value)](#setVertical-boolean-) | Verdadero si una fila en el archivo Workbook representa una fila en DataTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Este valor indica si se permiten DBNulls en esta tabla.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


Falso, Aspose.Cells establecerá el tipo de DataColumn por el tipo de valor de la primera fila para mejorar el rendimiento. Verdadero, Aspose.Cells comprobará si el tipo de valor en la columna está mezclado antes de establecer el tipo de DataColumn y, si los tipos de valor están mezclados, el tipo de DataColumn será cadena.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Exporta el valor de cadena html de las celdas al DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exporta el valor de cadena de las celdas al DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. El valor predeterminado es falso.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtiene la estrategia de formato al exportar el valor como cadena.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

El valor predeterminado es [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Los índices de columnas/filas que deben exportarse.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Solo exporta celdas visibles.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Solo exporta columnas visibles.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Solo exporta filas visibles.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Estrategia para nombres duplicados de columnas.

Ver [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Indica si se omite el valor inválido para la columna. Por ejemplo, si el tipo de columna es decimal, el valor es mayor que decimal.MaxValue y esta propiedad es verdadera, no lanzaremos la excepción nuevamente. El valor predeterminado es falso.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


Verdadero si una fila en el archivo Workbook representa una fila en DataTable. Falso si una columna en el archivo Workbook representa una fila en DataTable.

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




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Preprocesa el valor de la celda actual para exportarla.

**Remarks**

El índice de fila y columna es el índice absoluto de la celda en la hoja de cálculo, no el índice en la tabla exportada. El usuario puede comprobar el valor de la celda actual en la implementación sobrescrita de este método; si la celda actual necesita ser reemplazada por otro tipo y valor, aquí la implementación debe establecer el tipo y valor esperados en el objeto CellValue y devolver verdadero. Por defecto, este método no hace nada y devuelve falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellRow | int | el índice de fila de la celda actual |
| cellColumn | int | el índice de columna de la celda |
| value | [CellValue](../../com.aspose.cells/cellvalue) | valor y tipo de la celda actual |

**Returns:**
booleano - Indica si la celda actual ha sido reemplazada con un tipo y/o valor diferente.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Este valor indica si se permiten DBNulls en esta tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


Falso, Aspose.Cells establecerá el tipo de DataColumn por el tipo de valor de la primera fila para mejorar el rendimiento. Verdadero, Aspose.Cells comprobará si el tipo de valor en la columna está mezclado antes de establecer el tipo de DataColumn y, si los tipos de valor están mezclados, el tipo de DataColumn será cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Exporta el valor de cadena html de las celdas al DataTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exporta el valor de cadena de las celdas al DataTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Establece la estrategia de formato al exportar el valor como cadena.

Ver [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

El valor predeterminado es [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Los índices de columnas/filas que deben exportarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Solo exporta celdas visibles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Solo exporta columnas visibles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Solo exporta filas visibles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Estrategia para nombres duplicados de columnas.

Ver [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Indica si se omite el valor inválido para la columna. Por ejemplo, si el tipo de columna es decimal, el valor es mayor que decimal.MaxValue y esta propiedad es verdadera, no lanzaremos la excepción nuevamente. El valor predeterminado es falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


Verdadero si una fila en el archivo Workbook representa una fila en DataTable. Falso si una columna en el archivo Workbook representa una fila en DataTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

