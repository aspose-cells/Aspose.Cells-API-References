---
title: "ListObject"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una tabla en una hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Representa una tabla en una hoja de cálculo.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Aplica el estilo de tabla al rango. |
| [convertToRange()](#convertToRange--) | Convierte la tabla en rango. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Convierte la tabla en rango. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filtra la tabla. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Obtiene la descripción alternativa. |
| [getAlternativeText()](#getAlternativeText--) | Obtiene el texto alternativo. |
| [getAutoFilter()](#getAutoFilter--) | Obtiene el autofiltro de esta tabla. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Obtiene el comentario de la tabla. |
| [getDataRange()](#getDataRange--) | Obtiene el rango de datos de la Tabla. |
| [getDataSourceType()](#getDataSourceType--) | Obtiene el tipo de origen de datos de la tabla. |
| [getDisplayName()](#getDisplayName--) | Obtiene el nombre para mostrar de la tabla. |
| [getEndColumn()](#getEndColumn--) | Obtiene la columna final del rango. |
| [getEndRow()](#getEndRow--) | Obtiene la fila final del rango. |
| [getListColumns()](#getListColumns--) | Obtiene la lista [ListColumn](../../com.aspose.cells/listcolumn) de esta tabla. |
| [getQueryTable()](#getQueryTable--) | Obtiene la QueryTable vinculada. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Obtiene si esta Tabla muestra la fila de encabezado. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indica si se aplica formato de franjas de columna. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indica si la primera columna de la tabla tiene el estilo aplicado. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indica si la última columna de la tabla tiene el estilo aplicado. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indica si se aplica formato de franjas de fila. |
| [getShowTotals()](#getShowTotals--) | Obtiene si esta Tabla muestra la fila total. |
| [getStartColumn()](#getStartColumn--) | Obtiene la columna inicial del rango. |
| [getStartRow()](#getStartRow--) | Obtiene la fila inicial del rango. |
| [getTableStyleName()](#getTableStyleName--) | Obtiene el nombre del estilo de tabla. |
| [getTableStyleType()](#getTableStyleType--) | Obtiene el estilo de tabla incorporado. |
| [getXmlMap()](#getXmlMap--) | Obtiene un [getXmlMap()](../../com.aspose.cells/listobject\\#getXmlMap--) usado para esta lista. |
| [hasAutoFilter()](#hasAutoFilter--) | Indica si se aplica filtro automático a esta tabla. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Coloca la fórmula en la celda de la tabla. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Coloca la fórmula en la celda de la tabla. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Coloca el valor en la celda. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Coloca el valor en la celda. |
| [removeAutoFilter()](#removeAutoFilter--) | Elimina el filtro automático que se aplica a esta tabla. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Redimensiona el rango del objeto de lista. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Establece la descripción alternativa. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Establece el texto alternativo. |
| [setComment(String value)](#setComment-java.lang.String-) | Establece el comentario de la tabla. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Establece el nombre para mostrar de la tabla. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Indica si se aplica filtro automático a esta tabla. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Establece si esta Tabla muestra la fila de encabezado. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Indica si se aplica formato de franjas de columna. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Indica si la primera columna de la tabla tiene el estilo aplicado. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Indica si la última columna de la tabla tiene el estilo aplicado. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Indica si se aplica formato de franjas de fila. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Establece si esta TAble muestra la fila total. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Establece el nombre del estilo de tabla. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Obtiene el estilo de tabla incorporado. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Actualiza el nombre de todas las columnas de lista a celdas en la tabla. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Aplica el estilo de tabla al rango.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Convierte la tabla en rango.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Convierte la tabla en rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | las opciones al convertir la tabla a rango. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filtra la tabla.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor establezca la propiedad ListObject.HasAutoFilter./// Esta propiedad será eliminada 12 meses después desde octubre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Obtiene la descripción alternativa.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Obtiene el texto alternativo.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Obtiene el autofiltro de esta tabla.

**Remarks**

Solo funciona cuando [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) es falso.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Obtiene el comentario de la tabla.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Obtiene el rango de datos de la Tabla.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Obtiene el tipo de origen de datos de la tabla.

Ver [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Obtiene el nombre para mostrar de la tabla.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Obtiene la columna final del rango.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Obtiene la fila final del rango.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Obtiene la lista [ListColumn](../../com.aspose.cells/listcolumn) de esta tabla.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Obtiene la QueryTable vinculada.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Obtiene si esta Tabla muestra la fila de encabezado.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indica si se aplica formato de franjas de columna.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indica si la primera columna de la tabla tiene el estilo aplicado.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indica si la última columna de la tabla tiene el estilo aplicado.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indica si se aplica formato de franjas de fila.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Obtiene si esta Tabla muestra la fila total.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Obtiene la columna inicial del rango.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Obtiene la fila inicial del rango.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Obtiene el nombre del estilo de tabla.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Obtiene el estilo de tabla incorporado.

Ver [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Obtiene un [getXmlMap()](../../com.aspose.cells/listobject\\#getXmlMap--) usado para esta lista.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Indica si se aplica filtro automático a esta tabla.

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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Coloca la fórmula en la celda de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | El desplazamiento de fila en la tabla. |
| columnOffset | int | El desplazamiento de columna en la tabla. |
| formula | java.lang.String | La fórmula de la celda. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Coloca la fórmula en la celda de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | El desplazamiento de fila en la tabla. |
| columnOffset | int | El desplazamiento de columna en la tabla. |
| formula | java.lang.String | La fórmula de la celda. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Coloca el valor en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | El desplazamiento de fila en la tabla. |
| columnOffset | int | El desplazamiento de columna en la tabla. |
| valor | java.lang.Object | El valor de la celda. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Coloca el valor en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | El desplazamiento de fila en la tabla. |
| columnOffset | int | El desplazamiento de columna en la tabla. |
| valor | java.lang.Object | El valor de la celda. |
| isTotalsRowLabel | boolean | Indica si es una etiqueta para la fila total, solo funciona para la fila total. Si es False y esta fila es la fila total, se insertará una nueva fila. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Elimina el filtro automático que se aplica a esta tabla.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Redimensiona el rango del objeto de lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | El índice de fila inicial del nuevo rango. |
| startColumn | int | El índice de columna inicial del nuevo rango. |
| endRow | int | El índice de fila final del nuevo rango. |
| endColumn | int | El índice de columna final del nuevo rango. |
| hasHeaders | boolean | Si esta tabla tiene encabezados. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Establece la descripción alternativa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Establece el texto alternativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Establece el comentario de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Establece el nombre para mostrar de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Indica si se aplica filtro automático a esta tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Establece si esta Tabla muestra la fila de encabezado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Indica si se aplica formato de franjas de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Indica si la primera columna de la tabla tiene el estilo aplicado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Indica si la última columna de la tabla tiene el estilo aplicado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Indica si se aplica formato de franjas de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Establece si esta TAble muestra la fila total.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Establece el nombre del estilo de tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Obtiene el estilo de tabla incorporado.

Ver [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Actualiza el nombre de todas las columnas de lista a celdas en la tabla.

**Remarks**

El valor de las celdas en la fila de encabezado de la tabla debe ser el mismo que el nombre de la ListColumn; Cell.PutValue no modifica automáticamente el nombre de la ListColumn por rendimiento.

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

