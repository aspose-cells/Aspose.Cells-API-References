---
title: "PivotField"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un campo en un informe de tabla dinámica."
type: docs
url: /es/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Representa un campo en un informe de tabla dinámica.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Añade un elemento de fórmula calculada al pivot field. |
| [clearFilter()](#clearFilter--) | Borra la configuración de filtro en este pivot field. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtra por valores de fecha de la fila o columna del pivot field. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filtra por leyendas del campo pivot de fila o columna. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filtra por valores del campo pivot de datos. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filtra por valores del campo pivot de datos. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Indica si el campo especificado puede arrastrarse a la región de columna. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Indica si el campo especificado puede arrastrarse a la región de valores. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Indica si el campo especificado puede arrastrarse a la región de página. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Indica si el campo especificado puede arrastrarse a la región de fila. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Indica si este pivot field puede eliminarse de la vista de PivotTable. |
| [getAutoShowCount()](#getAutoShowCount--) | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [getAutoShowField()](#getAutoShowField--) | Representa el índice del campo de auto visualización. -1 significa el propio PivotField. |
| [getAutoSortField()](#getAutoSortField--) | Representa el índice del campo que está ordenado automáticamente. |
| [getBaseIndex()](#getBaseIndex--) | Representa el índice en los campos pivot de origen. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Obtén la cadena de fórmula del campo calculado especificado. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Obtiene el elemento de página actualmente mostrado para este pivot field (solo campo de página). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Obtiene el texto de visualización del elemento de página actual para este pivot field (solo campo de página). |
| [getDisplayName()](#getDisplayName--) | Representa el nombre de visualización del pivot field en la vista de la tabla dinámica. |
| [getDragToColumn()](#getDragToColumn--) | Indica si el campo especificado puede arrastrarse a la región de columna. |
| [getDragToData()](#getDragToData--) | Indica si el campo especificado puede arrastrarse a la región de valores. |
| [getDragToHide()](#getDragToHide--) | Indica si este pivot field puede eliminarse de la vista de PivotTable. |
| [getDragToPage()](#getDragToPage--) | Indica si el campo especificado puede arrastrarse a la región de página. |
| [getDragToRow()](#getDragToRow--) | Indica si el campo especificado puede arrastrarse a la región de fila. |
| [getFilters()](#getFilters--) | Obtiene todos los filtros pivot aplicados a este pivot field. |
| [getFormula()](#getFormula--) | Obtiene la fórmula del campo calculado. |
| [getFunction()](#getFunction--) | Representa la función utilizada para resumir este campo de datos de PivotTable. |
| [getGroupSettings()](#getGroupSettings--) | Obtiene la configuración de grupo del pivot field. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Indica si se debe insertar una línea en blanco después de cada elemento. |
| [getItemCount()](#getItemCount--) | Obtiene el recuento de los elementos base en este pivot field. |
| [getItems()](#getItems--) | Obtiene todas las etiquetas de los pivot items en este campo. |
| [getMaxValue()](#getMaxValue--) | Obtiene el valor máximo de este campo. |
| [getMinValue()](#getMinValue--) | Obtiene el valor máximo de este campo. |
| [getName()](#getName--) | Representa el nombre de PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple. |
| [getNumber()](#getNumber--) | Representa el formato de visualización incorporado de números y fechas. |
| [getNumberFormat()](#getNumberFormat--) | Representa el formato de visualización personalizado de números y fechas. |
| [getOriginalItems()](#getOriginalItems--) | Obtiene los elementos base originales; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Obtiene el filtro pivot del pivot field por tipo |
| [getPivotFilters()](#getPivotFilters--) | Obtiene los filtros pivot del pivot field |
| [getPivotItems()](#getPivotItems--) | Obtiene los pivot items del pivot field |
| [getPosition()](#getPosition--) | Representa el índice de [PivotField](../../com.aspose.cells/pivotfield) en la región. |
| [getRegionType()](#getRegionType--) | Especifica la región de la tabla dinámica donde se muestra este campo. |
| [getShowAllItems()](#getShowAllItems--) | Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. |
| [getShowCompact()](#getShowCompact--) | Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de la tabla dinámica. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Obtiene un valor que indica si este campo de fila utiliza el diseño de forma compacta. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Obtiene un valor que indica si este campo de fila utiliza el diseño de esquema. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Obtiene la configuración de mostrar valores como cuando se utiliza el cálculo ShowDataAs. |
| [getSortSetting()](#getSortSetting--) | Obtiene todas las configuraciones de ordenación automática |
| [getSubtotals()](#getSubtotals--) | Obtiene los subtotales del campo. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Indica si se debe mostrar el subtotal especificado para este campo dinámico. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Obtiene la configuración Top 10 AutoShow para un campo dinámico. |
| [group()](#group--) | Agrupa automáticamente el campo. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Agrupa el campo dinámico con opciones. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Agrupa el archivo por los tipos de grupo de fecha. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Agrupa el archivo por número. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Agrupa el campo de forma personalizada. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Agrupa el archivo por los tipos de grupo de fecha. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Agrupa el campo de forma personalizada. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Agrupa automáticamente el campo con intervalo |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Agrupa el archivo por número. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Agrupa automáticamente el campo con interno |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Oculta todos los detalles de cada elemento dinámico. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Establece si el detalle de todos los PivotItems en un campo dinámico está oculto. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Establece si el PivotItem específico en un campo de datos está oculto. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Establece si el PivotItem específico en un campo de datos está oculto. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Establece si el detalle del PivotItem específico en un campo dinámico está oculto. |
| [initPivotItems()](#initPivotItems--) | Inicializa los elementos dinámicos del campo dinámico. |
| [isAscendShow()](#isAscendShow--) | Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
| [isAscendSort()](#isAscendSort--) | Indica si los elementos de este campo dinámico están ordenados automáticamente de forma ascendente. |
| [isAutoShow()](#isAutoShow--) | Indica si el campo especificado de la tabla dinámica se muestra automáticamente. |
| [isAutoSort()](#isAutoSort--) | Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Indica si el campo especificado muestra subtotales automáticos. |
| [isCalculatedField()](#isCalculatedField--) | Indica si este campo dinámico es un campo calculado. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Indica si el PivotItem específico está oculto. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Indica si se debe ocultar el detalle del PivotItem específico. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Indica si se deben incluir nuevos elementos al campo en el filtro manual. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Indica si se deben insertar saltos de página después de cada elemento. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Indica si se pueden seleccionar varios elementos en el campo de página. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Indica si se deben repetir las etiquetas del campo en la región de filas o columnas. |
| [isValueFields()](#isValueFields--) | Indica si este campo representa campos de valores. |
| [isValuesField()](#isValuesField--) | Indica si este campo representa un campo de valores. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Indica si el campo especificado puede arrastrarse a la región de columna. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Indica si el campo especificado puede arrastrarse a la región de valores. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Indica si el campo especificado puede arrastrarse a la región de página. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Indica si el campo especificado puede arrastrarse a la región de fila. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Indica si este pivot field puede eliminarse de la vista de PivotTable. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indica si los elementos de este campo dinámico están ordenados automáticamente de forma ascendente. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indica si el campo especificado de la tabla dinámica se muestra automáticamente. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Representa el índice del campo de auto visualización. -1 significa el propio PivotField. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Representa el índice del campo que está ordenado automáticamente. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Indica si el campo especificado muestra subtotales automáticos. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Representa el índice en los campos pivot de origen. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Establece el elemento de página actualmente mostrado para este campo de tabla dinámica (solo campo de página). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Obtiene el texto de visualización del elemento de página actual para este pivot field (solo campo de página). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Representa el nombre de visualización del pivot field en la vista de la tabla dinámica. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Indica si el campo especificado puede arrastrarse a la región de columna. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Indica si el campo especificado puede arrastrarse a la región de valores. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Indica si este pivot field puede eliminarse de la vista de PivotTable. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Indica si el campo especificado puede arrastrarse a la región de página. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Indica si el campo especificado puede arrastrarse a la región de fila. |
| [setFunction(int value)](#setFunction-int-) | Representa la función utilizada para resumir este campo de datos de PivotTable. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Indica si se deben incluir nuevos elementos al campo en el filtro manual. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Indica si se debe insertar una línea en blanco después de cada elemento. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Indica si se deben insertar saltos de página después de cada elemento. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Indica si se pueden seleccionar varios elementos en el campo de página. |
| [setName(String value)](#setName-java.lang.String-) | Representa el nombre de PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple. |
| [setNumber(int value)](#setNumber-int-) | Representa el formato de visualización incorporado de números y fechas. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Representa el formato de visualización personalizado de números y fechas. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Indica si se deben repetir las etiquetas del campo en la región de filas o columnas. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de la tabla dinámica. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Establece un valor que indica si este campo de fila usa el diseño de forma compacta. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Establece un valor que indica si este campo de fila usa el diseño de esquema. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos. |
| [setSubtotals(int value)](#setSubtotals-int-) | Establece los subtotales del campo. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Establece cómo subtotalizar el campo especificado. |
| [showAllDetails()](#showAllDetails--) | Mostrar todos los detalles de cada elemento de tabla dinámica. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Establece el cálculo "Mostrar valores como" para este campo de tabla dinámica. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Muestra los valores del campo de datos en un formato de visualización diferente cuando se utiliza el cálculo MostrarDatosComo. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Configura el cálculo "Mostrar valores como" para este campo de datos. |
| [sortBy(int sortType)](#sortBy-int-) | Ordena este campo de tabla dinámica. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Ordena este campo de tabla dinámica. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Ordena este campo de tabla dinámica. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Ordena este campo de tabla dinámica. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Configura la configuración Top10 AutoShow para este campo de tabla dinámica. |
| [ungroup()](#ungroup--) | Desagrupar el campo de tabla dinámica. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Añade un elemento de fórmula calculada al pivot field.

**Remarks**

Solo admite agregar un elemento calculado al campo de fila/columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del elemento. |
| formula | java.lang.String | La fórmula del elemento de tabla dinámica. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Borra la configuración de filtro en este pivot field.

### dispose() {#dispose--}
```
public void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filtra por valores de fecha de la fila o columna del pivot field.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | La etiqueta de fecha de la condición de filtro |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | La etiqueta de fecha límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filtra por leyendas del campo pivot de fila o columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| label1 | java.lang.String | La etiqueta de la condición de filtro |
| label2 | java.lang.String | La etiqueta límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filtra por valores del campo pivot de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valueFieldIndex | int | El índice del campo de valor en la región de valores. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| value1 | double | El valor de la condición de filtro |
| value2 | double | El valor límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtra por valores del campo pivot de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valueFieldIndex | int | El índice del campo de datos en la región de datos. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. Solo puede ser Count,Sum y Percent. |
| isTop | boolean | Indica si el filtro es de arriba o de abajo |
| itemCount | int | El recuento de elementos |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Indica si este campo de tabla dinámica puede eliminarse de la vista de tabla dinámica. El valor predeterminado es verdadero.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.AutoShowCount o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Representa el índice del campo de auto‑mostrar. -1 significa el propio PivotField. Debe ser el índice de los campos de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.RankBy o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Representa el índice del campo que se ordena automáticamente. -1 significa el propio PivotField; otros valores indican la posición de los campos de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortBy o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Representa el índice en los campos pivot de origen.

**Remarks**

NOTA: Este setter de la propiedad está ahora obsoleto. Este setter será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Obtén la cadena de fórmula del campo calculado especificado.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.GetFormula(). Este método será eliminado 12 meses después, a partir de agosto de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Obtiene el elemento de página actualmente mostrado para este pivot field (solo campo de página).

**Remarks**

Utilice [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) como el valor centinela para indicar \"Seleccionar todo\". Este es un marcador predefinido y no es un índice de elemento válido.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Obtiene el texto de visualización del elemento de página actual para este pivot field (solo campo de página).

**Remarks**

Devuelve \"(All)\" cuando [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) es igual a [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). Para otros valores, devuelve la representación en cadena del índice del elemento.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Representa el nombre de visualización del pivot field en la vista de la tabla dinámica.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToColumn. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToData. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Indica si este campo de tabla dinámica puede eliminarse de la vista de tabla dinámica. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowRemovingFromView. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToPage. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToRow. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Obtiene todos los filtros pivot aplicados a este pivot field.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene la fórmula del campo calculado. Solo funciona para el campo calculado.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Representa la función utilizada para resumir este campo de datos de PivotTable.

Consulte [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Obtiene la configuración de grupo del pivot field.

**Remarks**

Si este campo no está agrupado, se devolverá Null.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Indica si se debe insertar una línea en blanco después de cada elemento. Solo para campos de fila.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Obtiene el recuento de los elementos base en este pivot field.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems.Count. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Obtiene todas las etiquetas de los pivot items en este campo.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Obtiene el valor máximo de este campo.

**Remarks**

Solo funciona para campos de fila o columna cuyo valor debe ser fecha y hora, número o vacío.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Obtiene el valor máximo de este campo.

**Remarks**

Solo funciona para campos de fila o columna cuyo valor debe ser fecha y hora, número o vacío.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Representa el nombre de PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad !PivotField.SortSetting.IsSimpleSort. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Representa el formato de visualización incorporado de números y fechas.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Representa el formato de visualización personalizado de números y fechas.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Obtiene los elementos base originales;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Obtiene el filtro pivot del pivot field por tipo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Obtiene los filtros pivot del pivot field

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.GetFilters() method. Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Obtiene los pivot items del pivot field

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Representa el índice de [PivotField](../../com.aspose.cells/pivotfield) en la región.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Especifica la región de la tabla dinámica donde se muestra este campo.

Ver [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. El valor predeterminado es false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de Pivot Table. Solo para campos de fila.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.ShowInCompactForm property instead . Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Obtiene un valor que indica si este campo de fila utiliza el diseño de forma compacta. Solo se aplica a campos de fila.

**Remarks**

La forma compacta es un submodo del diseño de esquema. Esta configuración solo tiene efecto cuando [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) es true.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Obtiene un valor que indica si este campo de fila utiliza el diseño de esquema. Solo se aplica a campos de fila.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos.

**Remarks**

Solo funciona para los campos de pivote en la región de fila cuando ShowInOutlineForm es true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Obtiene la configuración de mostrar valores como cuando se utiliza el cálculo ShowDataAs.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Obtiene todas las configuraciones de ordenación automática

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Obtiene los subtotales del campo. Solo para campos de pivote de fila o columna.

Ver [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Indica si se debe mostrar el subtotal especificado para este campo dinámico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Tipo de subtotal. |

**Returns:**
boolean - Devuelve si se muestra el subtotal especificado.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Obtiene la configuración Top 10 AutoShow para un campo dinámico.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Agrupa automáticamente el campo.

**Remarks**

Si el campo solo contiene valores en blanco y fecha/hora, el campo se agrupará por Meses. Si el campo solo contiene valores en blanco y número, el campo se agrupará por Número. De lo contrario, solo devuelve false sin ningún grupo.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Agrupa el campo dinámico con opciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Opciones para la configuración de agrupación de campos de tabla dinámica. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Agrupa el archivo por los tipos de grupo de fecha.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoStart | boolean | Indica si se debe detectar automáticamente el valor de fecha y hora de inicio. |
| start | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de inicio |
| isAutoEnd | boolean | Indica si se debe detectar automáticamente el valor de fecha y hora de fin. |
| end | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de fin |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipos de grupo |
| interval | double | El intervalo |
| firstAsNewField | boolean | Indica si se agrega un nuevo campo a la tabla dinámica. Solo para el primer elemento del grupo. |

**Returns:**
boolean - False significa que este campo no pudo ser agrupado por fecha y hora.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Agrupa el archivo por número.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoStart | boolean | Indica si se debe detectar automáticamente el valor de inicio. |
| inicio | double | El valor de inicio |
| isAutoEnd | boolean | Indica si se debe detectar automáticamente el valor final. |
| fin | double | El final del valor |
| interval | double | El intervalo |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica |

**Returns:**
boolean - False significa que este campo no pudo ser agrupado por fecha y hora.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Agrupa el campo de forma personalizada.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions options) con la propiedad PivotFieldGroupOptions.DiscreteGroupItems. Este método será eliminado 6 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Los elementos de grupo personalizados. |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica |

**Returns:**
boolean - False significa que este campo no pudo ser agrupado por fecha y hora.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Agrupa el archivo por los tipos de grupo de fecha.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de inicio |
| end | [DateTime](../../com.aspose.cells/datetime) | La fecha y hora de fin |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipos de grupo |
| interval | double | El intervalo |
| firstAsNewField | boolean | Indica si se agrega un nuevo campo a la tabla dinámica. Solo para el primer elemento del grupo. |

**Returns:**
boolean - False significa que este campo no pudo ser agrupado por fecha y hora.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Agrupa el campo de forma personalizada.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions options) con la propiedad PivotFieldGroupOptions.DiscreteGroupItems. Este método será eliminado 6 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Los elementos de grupo personalizados. |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Agrupa automáticamente el campo con intervalo

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| interval | double | El interno del grupo. Se asignará un valor automático si es cero, |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica. Sólo para el grupo DateTime. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Agrupa el archivo por número.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | double | El valor de inicio |
| fin | double | El final del valor |
| interval | double | El intervalo |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica |

**Returns:**
boolean - False significa que este campo no pudo ser agrupado por fecha y hora.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Agrupa automáticamente el campo con interno

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions) method . Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipos de grupo |
| interval | double | El interno del grupo. Se asignará un valor automático si es cero, sólo funciona para agrupar por Números o Días. |
| newField | boolean | Indica si se está añadiendo un nuevo campo a la tabla dinámica. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Oculta todos los detalles de cada elemento dinámico.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Establece si el detalle de todos los PivotItems en un campo dinámico está oculto. Es decir, colapsar/expandir este campo.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice los métodos PivotItemsCollection.HideAllDetails() y UnhideAllDetails(). Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isHiddenDetail | boolean | Si oculta el detalle del pivot field. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Establece si el PivotItem específico en un campo de datos está oculto.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del pivotItem en el pivotField. |
| isHidden | boolean | si el PivotItem específico está oculto |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Establece si el PivotItem específico en un campo de datos está oculto.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[string].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| itemValue | java.lang.String | El nombre del pivotItem en el pivotField. |
| isHidden | boolean | Si el PivotItem específico está oculto |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Establece si el detalle del PivotItem específico en un campo dinámico está oculto.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsDetailHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del pivotItem en el pivotField. |
| isHiddenDetail | boolean | si el PivotItem específico está oculto |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Inicializa los elementos dinámicos del campo dinámico.

**Remarks**

NOTA: Este método está ahora obsoleto. Simplemente elimine la llamada a este método. Este método será eliminado 6 meses después, a partir de octubre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsTop o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Indica si los elementos de este campo dinámico están ordenados automáticamente de forma ascendente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortType o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indica si el campo especificado de la tabla dinámica se muestra automáticamente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsAutoShow o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortType o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Indica si este campo dinámico es un campo calculado.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Indica si el PivotItem específico está oculto.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del pivotItem en el pivotField. |

**Returns:**
boolean - si el PivotItem específico está oculto
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Indica si se debe ocultar el detalle del PivotItem específico.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsDetailHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del pivotItem en el pivotField. |

**Returns:**
boolean - si el detalle oculto del PivotItem específico
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Indica si se deben incluir nuevos elementos al campo en el filtro manual. El valor predeterminado es false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Indica si se deben insertar saltos de página después de cada elemento. El valor predeterminado es false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es false.

**Remarks**

Solo para campos de página (filtro).

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Indica si se deben repetir las etiquetas del campo en la región de fila o columna. El valor predeterminado es false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Indica si este campo representa campos de valores.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.IsValuesField. Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Indica si este campo representa un campo de valores.

**Remarks**

Solo funciona cuando hay dos o más campos de datos en la vista de tabla dinámica.

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




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Indica si este campo de tabla dinámica puede eliminarse de la vista de tabla dinámica. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsTop o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Indica si los elementos de este campo dinámico están ordenados automáticamente de forma ascendente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortType o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indica si el campo especificado de la tabla dinámica se muestra automáticamente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsAutoShow o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.AutoShowCount o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Representa el índice del campo de auto‑mostrar. -1 significa el propio PivotField. Debe ser el índice de los campos de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.RankBy o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortType o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Representa el índice del campo que se ordena automáticamente. -1 significa el propio PivotField; otros valores indican la posición de los campos de datos.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortBy o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Representa el índice en los campos pivot de origen.

**Remarks**

NOTA: Este setter de la propiedad está ahora obsoleto. Este setter será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Establece el elemento de página actualmente mostrado para este campo de tabla dinámica (solo campo de página).

**Remarks**

Utilice [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) como el valor centinela para indicar \"Seleccionar todo\". Este es un marcador predefinido y no es un índice de elemento válido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Obtiene el texto de visualización del elemento de página actual para este pivot field (solo campo de página).

**Remarks**

Devuelve \"(All)\" cuando [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) es igual a [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). Para otros valores, devuelve la representación en cadena del índice del elemento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Representa el nombre de visualización del pivot field en la vista de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToColumn. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToData. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Indica si este campo de tabla dinámica puede eliminarse de la vista de tabla dinámica. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowRemovingFromView. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToPage. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.AllowDraggingToRow. Este método será eliminado 12 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Representa la función utilizada para resumir este campo de datos de PivotTable.

Consulte [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Indica si se deben incluir nuevos elementos al campo en el filtro manual. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Indica si se debe insertar una línea en blanco después de cada elemento. Solo para campos de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Indica si se deben insertar saltos de página después de cada elemento. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es false.

**Remarks**

Solo para campos de página (filtro).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Representa el nombre de PivotField.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad !PivotField.SortSetting.IsSimpleSort. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Representa el formato de visualización incorporado de números y fechas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Representa el formato de visualización personalizado de números y fechas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Indica si se deben repetir las etiquetas del campo en la región de fila o columna. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de Pivot Table. Solo para campos de fila.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.ShowInCompactForm property instead . Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Establece un valor que indica si este campo de fila utiliza el diseño de forma compacta. Solo se aplica a los campos de fila.

**Remarks**

La forma compacta es un submodo del diseño de esquema. Esta configuración solo tiene efecto cuando [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Establece un valor que indica si este campo de fila utiliza el diseño de esquema. Solo se aplica a los campos de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos.

**Remarks**

Solo funciona para los campos de pivote en la región de fila cuando ShowInOutlineForm es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Establece los subtotales del campo. Solo para campos de fila o columna de tabla dinámica.

Ver [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Establece cómo subtotalizar el campo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| mostrado | boolean | Si el campo especificado muestra esos subtotales. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Mostrar todos los detalles de cada elemento de tabla dinámica.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Establece el cálculo "Mostrar valores como" para este campo de tabla dinámica.

**Remarks**

Solo para campo de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Tipo del cálculo "Mostrar valores como". |
| baseField | int | Índice del campo base utilizado para el cálculo. |
| baseItem | int | Índice del elemento base para el cálculo. Use [PivotShowValuesSetting.PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) para el elemento anterior, [PivotShowValuesSetting.NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) para el elemento siguiente; los valores non\\u9225\\u6182egative denotan el índice ordinal de un elemento pivot específico. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Muestra los valores del campo de datos en un formato de visualización diferente cuando se utiliza el cálculo MostrarDatosComo.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). El tipo de formato de visualización de datos. |
| baseField | int | El índice al campo en el que se basa el cálculo ShowDataAs. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). El tipo de posición del elemento base. |
| baseItem | int | El índice al elemento base en el que se basa el cálculo ShowDataAs. Solo funciona cuando baseItemPositionType es personalizado. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Configura el cálculo "Mostrar valores como" para este campo de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). El tipo de cálculo para Show Values As. |
| baseField | java.lang.String | El nombre del campo base utilizado en el cálculo. |
| baseItem | java.lang.String | Título de un elemento pivot regular. También acepta palabras clave literales reservadas: `(previous)` para el elemento anterior, `(next)` para el siguiente elemento. Pase `null` si el tipo de cálculo seleccionado no requiere un elemento base. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Ordena este campo de tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). El tipo de ordenación de este campo. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Ordena este campo de tabla dinámica.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.SortBy(SortOrder, int,string) o la propiedad PivotField.IsAutoSort. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). El tipo de ordenación de este campo. |
| fieldSortedBy | int | El índice del campo pivot por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Ordena este campo de tabla dinámica.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.SortBy(SortOrder, int,string). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). El tipo de ordenación de este campo. |
| fieldSortedBy | int | El índice del campo pivot por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). El tipo de datos por los que se ordena. |
| cellName | java.lang.String | Ordenar por valores en la fila o columna |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Ordena este campo de tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). El tipo de ordenación de este campo. |
| fieldSortedBy | int | El índice del campo pivot por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |
| cellName | java.lang.String | Ordenar por valores en la fila o columna. Si Null, agrupar por el total del campo; de lo contrario, agrupar por valores en la columna o fila seleccionada. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Configura la configuración Top10 AutoShow para este campo de tabla dinámica.

**Remarks**

Este método configura el formato binario .XLS: AutoShow (Top10) es la opción nativa y única admitida. XLSX (OpenXML): El formato de archivo subyacente admite Top10 AutoShow, pero la interfaz de usuario de Excel 2007 y posteriores solo lo expone mediante el filtro Top10. Si no se requiere compatibilidad con XLS, se recomienda usar el filtro Top10 en su lugar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoShow | boolean | true para habilitar AutoShow; false para deshabilitar. |
| isTop | boolean | Si es true, muestra los elementos superiores; false muestra los elementos inferiores. |
| recuento | int | Número de elementos superiores/inferiores a mostrar. |
| rankBy | int | Índice del campo de datos utilizado para la clasificación. Use -1 para clasificar por los propios valores del elemento pivot. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Desagrupar el campo de tabla dinámica.

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

