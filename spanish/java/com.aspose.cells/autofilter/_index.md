---
title: "AutoFilter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el autofiltro para la hoja de cálculo especificada."
type: docs
url: /es/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Representa el autofiltro para la hoja de cálculo especificada.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Agrega un filtro de fecha. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Agrega un filtro de color de relleno. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Agrega un filtro para una columna de filtro. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Agrega un filtro de color de fuente. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Agrega un filtro de ícono. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filtra una lista con un criterio personalizado. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtra una lista con criterios personalizados. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Agrega un filtro dinámico. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filtra una lista con criterios especificados. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filtrar los 10 elementos principales de la lista |
| [getCellArea()](#getCellArea--) | Obtiene el [CellArea](../../com.aspose.cells/cellarea) donde se aplica este AutoFilter. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Obtiene el [CellArea](../../com.aspose.cells/cellarea) donde se aplica el AutoFilter especificado. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Obtiene la colección de las columnas de filtro. |
| [getRange()](#getRange--) | Representa el rango al que se aplica el AutoFilter especificado. |
| [getShowFilterButton()](#getShowFilterButton--) | Indica si el botón AutoFilter para esta columna es visible. |
| [getSorter()](#getSorter--) | Obtiene el orden de los datos. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Coincide con todas las celdas en blanco de la lista. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Coincide con todas las celdas que no están en blanco de la lista. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualiza los filtros automáticos para ocultar o mostrar las filas. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Obtiene los índices de todas las filas ocultas. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Elimina un filtro de fecha. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Elimina el filtro específico. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Elimina un filtro para una columna de filtro. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Establece el rango al que se aplica el AutoFilter especificado. |
| [setRange(String value)](#setRange-java.lang.String-) | Representa el rango al que se aplica el AutoFilter especificado. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Indica si el botón AutoFilter para esta columna es visible. |
| [showAll()](#showAll--) | Desocultar todas las filas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Agrega un filtro de fecha.

**Remarks**

Si DateTimeGroupingType es Year, solo afecta el parámetro año. Si DateTiemGroupingType es Month, solo afectan los parámetros año y mes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). El tipo de agrupación |
| año | int | El año. |
| mes | int | El mes. |
| día | int | El día. |
| hora | int | La hora. |
| minuto | int | El minuto. |
| segundo | int | El segundo. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Agrega un filtro de color de relleno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). El tipo de patrón de fondo. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | El color de primer plano. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | El color de fondo. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Agrega un filtro para una columna de filtro.

**Remarks**

MS Excel 2007 admite selección múltiple en una columna de filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterios | java.lang.String | El criterio especificado (una cadena; por ejemplo, "101"). Sólo puede ser nulo o uno de los valores de celda en esta columna. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Agrega un filtro de color de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | El objeto [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Agrega un filtro de ícono.

**Remarks**

Sólo admite agregar el filtro de iconos. No admite comprobar qué fila está visible si el filtro es de iconos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). El tipo de conjunto de iconos. |
| iconId | int | El id del icono. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filtra una lista con un criterio personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). El tipo de operador de filtro |
| criteria1 | java.lang.Object | El criterio personalizado |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtra una lista con criterios personalizados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). El tipo de operador de filtro |
| criteria1 | java.lang.Object | El criterio personalizado |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). El tipo de operador de filtro |
| criteria2 | java.lang.Object | El criterio personalizado |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Agrega un filtro dinámico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Tipo de filtro dinámico. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filtra una lista con criterios especificados.

**Remarks**

Aspose.Cells eliminará todas las demás configuraciones de filtro en este campo como MS Excel 97-2003.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterios | java.lang.String | El criterio especificado (una cadena; por ejemplo, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filtrar los 10 elementos principales de la lista

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| isTop | boolean | Indica si el filtro es de arriba o de abajo |
| isPercent | boolean | Indica si los elementos son porcentaje o recuento |
| itemCount | int | El recuento de elementos |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtiene el [CellArea](../../com.aspose.cells/cellarea) donde se aplica este AutoFilter.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Obtiene el [CellArea](../../com.aspose.cells/cellarea) donde se aplica el AutoFilter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| refreshAppliedRange | boolean | Indica si se actualiza el rango aplicado. Para el rango aplicado del filtro automático, la última fila puede cambiar cuando los datos de las celdas cambian. Si este indicador es verdadero, la última fila del rango se recalculará según los datos actuales de las celdas. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Obtiene la colección de las columnas de filtro.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Representa el rango al que se aplica el AutoFilter especificado.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Indica si el botón AutoFilter para esta columna es visible.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Obtiene el orden de los datos.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Coincide con todas las celdas en blanco de la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Coincide con todas las celdas que no están en blanco de la lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Actualiza los filtros automáticos para ocultar o mostrar las filas.

**Returns:**
int[] - Devuelve los índices de todas las filas ocultas.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Obtiene los índices de todas las filas ocultas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hideRows | boolean | Si es verdadero, oculta las filas filtradas. |

**Returns:**
int[] - Devuelve los índices de todas las filas ocultas.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Elimina un filtro de fecha.

**Remarks**

Si DateTimeGroupingType es Year, solo afecta el parámetro año. Si DateTiemGroupingType es Month, solo afectan los parámetros año y mes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). El tipo de agrupación |
| año | int | El año. |
| mes | int | El mes. |
| día | int | El día. |
| hora | int | La hora. |
| minuto | int | El minuto. |
| segundo | int | El segundo. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Elimina el filtro específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El índice de filtro específico |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Elimina un filtro para una columna de filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | El desplazamiento entero del campo en el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| criterios | java.lang.String | El criterio especificado (una cadena; por ejemplo, "101"). Sólo puede ser nulo o uno de los valores de celda en esta columna. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Establece el rango al que se aplica el AutoFilter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Representa el rango al que se aplica el AutoFilter especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Indica si el botón AutoFilter para esta columna es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Desocultar todas las filas.

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

