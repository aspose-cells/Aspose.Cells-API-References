---
title: "Tabla dinámica"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Descripción resumida para PivotTable."
type: docs
url: /es/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Descripción resumida para PivotTable.

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
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Agrega un campo calculado al campo dinámico y lo arrastra al área de datos. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Agrega un campo calculado al campo dinámico. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Agrega el campo al área específica. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Agrega el campo al área específica. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Agrega el campo al área específica. |
| [calculateData()](#calculateData--) | Calcula los datos de la tabla dinámica a celdas. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Calcula la tabla dinámica con opciones. |
| [calculateRange()](#calculateRange--) | Calcula el rango de la tabla dinámica. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Cambiar la fuente de datos de la tabla dinámica. |
| [clearAll()](#clearAll--) | Eliminar todos los campos de las regiones. |
| [clearData()](#clearData--) | Borrar datos y formato de la vista de la tabla dinámica. |
| [clearFilters()](#clearFilters--) | Borra todos los filtros de esta tabla dinámica. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Copia el estilo con nombre de otra tabla dinámica. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Exporta la vista de tabla dinámica como JSON. |
| [fields(int fieldType)](#fields-int-) | Obtiene los campos específicos por el tipo de campo. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Da formato al área seleccionada de la tabla dinámica. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Da formato al área seleccionada de la tabla dinámica. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Da formato a la celda en el área de la tabla dinámica. |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Da formato a todas las celdas en el área de la tabla dinámica. |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Da formato a los datos de fila en el área de la tabla dinámica. |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [getAltTextDescription()](#getAltTextDescription--) | Obtiene la descripción del texto alternativo. |
| [getAltTextTitle()](#getAltTextTitle--) | Obtiene el título del texto alternativo. |
| [getAutoFormatType()](#getAutoFormatType--) | Obtiene el tipo de formato automático de la tabla dinámica. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Indica si ajustar automáticamente el ancho de columna al actualizar. |
| [getBaseFields()](#getBaseFields--) | Devuelve todos los campos base de la tabla dinámica. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Obtiene el área que contiene el botón de campo. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Obtiene el objeto [Cell](../../com.aspose.cells/cell) por el nombre para mostrar del PivotField. |
| [getChildren()](#getChildren--) | Obtiene las tablas dinámicas hijas que utilizan los datos de esta tabla dinámica como fuente de datos. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Devuelve un objeto PivotFields que se muestra actualmente como campos de columna. |
| [getColumnGrand()](#getColumnGrand--) | Indica si el informe de tabla dinámica muestra totales generales para las columnas. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Obtiene el título personalizado del encabezado de columna de la tabla dinámica. |
| [getColumnRange()](#getColumnRange--) | Devuelve un objeto CellArea que representa el rango que contiene el área de columnas en el informe de tabla dinámica. |
| [getConditionalFormats()](#getConditionalFormats--) | Obtiene los formatos condicionales de la tabla dinámica. |
| [getCustomListSort()](#getCustomListSort--) | Indica si se considera la lista personalizada incorporada al ordenar datos. |
| [getDataBodyRange()](#getDataBodyRange--) | Devuelve un objeto [CellArea](../../com.aspose.cells/cellarea) que representa el rango que contiene el área de datos en la lista entre la fila de encabezado y la fila de inserción. |
| [getDataField()](#getDataField--) | Obtiene un objeto [PivotField](../../com.aspose.cells/pivotfield) que representa todos los campos de datos en una tabla dinámica. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Obtiene el nombre del encabezado del campo del área de valores en la tabla dinámica. |
| [getDataFields()](#getDataFields--) | Obtiene una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que representa todos los campos de datos en una tabla dinámica. |
| [getDataSource()](#getDataSource--) | Obtiene la fuente de datos de la tabla dinámica. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Obtiene todas las [PivotTable](../../com.aspose.cells/pivottable)s que usan esta tabla dinámica como su fuente de datos. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Indica si el informe de la tabla dinámica muestra una cadena personalizada en celdas que contienen errores. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la tabla dinámica está vacía. |
| [getDisplayNullString()](#getDisplayNullString--) | Indica si el informe de la tabla dinámica muestra una cadena personalizada si el valor es nulo. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Especifica un valor booleano que indica si el usuario tiene permiso para editar las celdas en el área de datos de la tabla dinámica. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Indica si la perforación (drilldown) está habilitada. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Indica si el cuadro de diálogo de campo de tabla dinámica está disponible cuando el usuario hace doble clic en el campo de la tabla dinámica. |
| [getEnableFieldList()](#getEnableFieldList--) | Indica si la lista de campos para la tabla dinámica está disponible en la vista de Excel. |
| [getEnableWizard()](#getEnableWizard--) | Indica si el Asistente de tabla dinámica está disponible. |
| [getErrorString()](#getErrorString--) | Obtiene la cadena mostrada en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Obtiene la fuente de datos de la conexión externa. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Indica si los campos en la tabla dinámica están ordenados en un orden no predeterminado en la lista de campos. |
| [getFields(int fieldType)](#getFields-int-) | Obtiene la lista de campos de tabla dinámica específica por la región. |
| [getFilterArea()](#getFilterArea--) | Obtiene el área de la región de filtro. |
| [getGrandTotalName()](#getGrandTotalName--) | Devuelve la etiqueta que se muestra en el encabezado de columna o fila del total general. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Obtiene la lista de índices de fila de la tabla dinámica de saltos de página horizontales |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Obtiene los saltos de página horizontales de esta tabla dinámica. |
| [getIndent()](#getIndent--) | Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en Forma Compacta. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa. |
| [getManualUpdate()](#getManualUpdate--) | Indica si el informe de la tabla dinámica se recalcula solo a solicitud del usuario. |
| [getMergeLabels()](#getMergeLabels--) | Obtiene si se deben combinar las etiquetas de campo de fila/columna que abarcan varias celdas. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [getName()](#getName--) | Obtiene el nombre de la tabla dinámica |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Obtiene los nombres de las conexiones de datos de origen externo. |
| [getNullString()](#getNullString--) | Obtiene la cadena mostrada en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Obtiene el orden en que los campos de página se añaden al diseño del informe de tabla dinámica. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Obtiene el número de campos de página en cada columna o fila del informe de tabla dinámica. |
| [getPageFields()](#getPageFields--) | Devuelve una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que se muestra actualmente como campos de página. |
| [getPivotCache()](#getPivotCache--) | Obtiene la fuente de datos. |
| [getPivotFilters()](#getPivotFilters--) | Devuelve todos los filtros en la tabla dinámica. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Obtiene las condiciones de formato de la tabla dinámica. |
| [getPivotFormats()](#getPivotFormats--) | Obtiene todos los formatos de celda aplicados a esta tabla dinámica. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Obtiene la configuración de [TableStyle](../../com.aspose.cells/tablestyle) de esta tabla dinámica. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Obtiene el nombre del estilo de la tabla dinámica. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Obtiene el estilo incorporado de la tabla dinámica. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Obtiene todas las tablas dinámicas con la misma caché de tabla dinámica. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Indica si se debe preservar el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) cuando la tabla dinámica se actualiza o recalcula. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Indica si el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) se preserva cuando la tabla dinámica se actualiza o recalcula. |
| [getPrintDrill()](#getPrintDrill--) | Especifica un valor booleano que indica si los indicadores de desglose deben imprimirse. |
| [getPrintTitles()](#getPrintTitles--) | Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de tabla dinámica. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Indica si se deben actualizar los datos al abrir el archivo. |
| [getRefreshDate()](#getRefreshDate--) | Obtiene la fecha y hora de la última actualización de la tabla dinámica. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Obtiene el nombre del último usuario que actualizó esta tabla dinámica |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular. |
| [getRowFields()](#getRowFields--) | Devuelve una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que se muestra actualmente como campos de fila. |
| [getRowGrand()](#getRowGrand--) | Indica si se deben mostrar los totales generales para las filas de esta tabla dinámica. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Obtiene el título personalizado del encabezado de fila en esta tabla dinámica. |
| [getRowRange()](#getRowRange--) | Devuelve un objeto CellArea que representa el rango que contiene el área de filas en el informe de tabla dinámica. |
| [getSaveData()](#getSaveData--) | Indica si los datos del informe de PivotTable se guardan con el libro. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Indica si se deben mostrar los totales generales para las columnas de esta PivotTable. |
| [getShowDataTips()](#getShowDataTips--) | Indica si se deben mostrar descripciones emergentes para las celdas de datos de PivotTable. |
| [getShowDrill()](#getShowDrill--) | Obtiene si se muestran los botones de expandir/contraer. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Indica si se deben incluir columnas vacías en la tabla |
| [getShowEmptyRow()](#getShowEmptyRow--) | Indica si se deben incluir filas vacías en la tabla. |
| [getShowHeaders()](#getShowHeaders--) | Indica si se deben mostrar los títulos de los campos de datos y los títulos de los campos de pivote en el eje de filas y el eje de columnas en la vista de PivotTable. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Especifica un valor booleano que indica si la información de propiedades de miembros debe omitirse de las descripciones emergentes de PivotTable. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Indica si el encabezado de columna en la PivotTable debe tener aplicado el estilo. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Indica si se aplica formato de franjas a la columna. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Indica si se aplica el formato de columna. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Indica si el encabezado de fila en la PivotTable debe tener aplicado el estilo. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Indica si se aplica formato de franjas a las filas. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Indica si se deben mostrar los totales generales para las filas de la PivotTable. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Indica si el título del encabezado de fila se muestra en el informe de PivotTable Indica si se muestran los títulos de los campos de visualización y los menús desplegables de filtro |
| [getShowValuesRow()](#getShowValuesRow--) | Indica si se muestra la fila de valores. |
| [getSource()](#getSource--) | Obtén la fuente de datos de esta PivotTable. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Obtén la fuente de datos de esta PivotTable. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Obtiene las fuentes de datos de conexión externa. |
| [getSourceType()](#getSourceType--) | Obtiene el tipo de fuente de datos de la PivotTable. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Indica si los elementos de campo de página ocultos en el informe de PivotTable se incluyen en los subtotales de filas y columnas, totales de bloque y totales generales. |
| [getTableRange1()](#getTableRange1--) | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de PivotTable, pero no incluye los campos de página. |
| [getTableRange2()](#getTableRange2--) | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de PivotTable, incluye los campos de página. |
| [getTag()](#getTag--) | Obtiene una cadena definida por el usuario que está asociada con esta vista de PivotTable. |
| [getTopRightArea()](#getTopRightArea--) | Representa el área en blanco en la esquina superior derecha de la PivotTable (esquina superior izquierda para hojas RTL). |
| [getValuesField()](#getValuesField--) | Obtiene un objeto [PivotField](../../com.aspose.cells/pivotfield) que representa todos los campos de datos en una tabla dinámica. |
| [hasBlankRows()](#hasBlankRows--) | Indica si se deben agregar filas en blanco. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Indica si el informe de tabla dinámica se formatea automáticamente. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Especifica si la tabla dinámica es compatible con Excel2003 al actualizarla; si es verdadero, una cadena debe tener como máximo 255 caracteres, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, una cadena no tendrá la restricción mencionada. |
| [isGridDropZones()](#isGridDropZones--) | Indica si el informe de tabla dinámica muestra el diseño clásico de tabla dinámica. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [isSelected()](#isSelected--) | Indica si esta tabla dinámica está seleccionada. |
| [move(int row, int column)](#move-int-int-) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [move(String destCellName)](#move-java.lang.String-) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Mueve un elemento hacia arriba o hacia abajo. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Actualiza [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Actualiza [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica. |
| [refreshData()](#refreshData--) | Actualiza los datos desde su fuente de datos al caché de tabla dinámica. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos con opciones. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Eliminar campo del área de campo específica |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Elimina un campo de una región de tabla dinámica específica. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Elimina un campo del área de campo específica. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Selecciona un área de la vista de tabla dinámica. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Obtiene la descripción del texto alternativo. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Establece el título del texto alternativo. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Indica si el informe de tabla dinámica se formatea automáticamente. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Establece el tipo de formato automático de la tabla dinámica. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Indica si ajustar automáticamente el ancho de columna al actualizar. |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Indica si el informe de tabla dinámica muestra totales generales para las columnas. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Establece el título personalizado del encabezado de columna de la tabla dinámica. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Indica si se considera la lista personalizada incorporada al ordenar datos. |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Establece el nombre del encabezado del campo del área de valores en la tabla dinámica. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Establece la fuente de datos de la tabla dinámica. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Indica si el informe de la tabla dinámica muestra una cadena personalizada en celdas que contienen errores. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la tabla dinámica está vacía. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Indica si el informe de la tabla dinámica muestra una cadena personalizada si el valor es nulo. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Especifica un valor booleano que indica si el usuario tiene permiso para editar las celdas en el área de datos de la tabla dinámica. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Indica si la perforación (drilldown) está habilitada. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Indica si el cuadro de diálogo de campo de tabla dinámica está disponible cuando el usuario hace doble clic en el campo de la tabla dinámica. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Indica si la lista de campos para la tabla dinámica está disponible en la vista de Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Indica si el Asistente de tabla dinámica está disponible. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Obtiene la cadena mostrada en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Especifica si la tabla dinámica es compatible con Excel2003 al actualizarla; si es verdadero, una cadena debe tener como máximo 255 caracteres, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, una cadena no tendrá la restricción mencionada. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Indica si los campos en la tabla dinámica están ordenados en un orden no predeterminado en la lista de campos. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Devuelve la etiqueta que se muestra en el encabezado de columna o fila del total general. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Indica si el informe de tabla dinámica muestra el diseño clásico de tabla dinámica. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Indica si se deben agregar filas en blanco. |
| [setIndent(int value)](#setIndent-int-) | Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en Forma Compacta. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Indica si el informe de la tabla dinámica se recalcula solo a solicitud del usuario. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Establece si se deben combinar las etiquetas de campo de fila/columna que abarcan varias celdas. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados. |
| [setName(String value)](#setName-java.lang.String-) | Obtiene el nombre de la tabla dinámica |
| [setNullString(String value)](#setNullString-java.lang.String-) | Obtiene la cadena mostrada en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Establece el orden en que los campos de página se añaden al diseño del informe de tabla dinámica. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Obtiene el número de campos de página en cada columna o fila del informe de tabla dinámica. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Obtiene la configuración de [TableStyle](../../com.aspose.cells/tablestyle) de esta tabla dinámica. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Establece el nombre del estilo de la tabla dinámica. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Establece el estilo incorporado de la tabla dinámica. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Indica si se debe preservar el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) cuando la tabla dinámica se actualiza o recalcula. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Indica si el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) se preserva cuando la tabla dinámica se actualiza o recalcula. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Especifica un valor booleano que indica si los indicadores de desglose deben imprimirse. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de tabla dinámica. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Indica si se deben actualizar los datos al abrir el archivo. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Indica si se deben mostrar los totales generales para las filas de esta tabla dinámica. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Establece el título personalizado del encabezado de fila en esta tabla dinámica. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Indica si los datos del informe de PivotTable se guardan con el libro. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica si esta tabla dinámica está seleccionada. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Indica si se deben mostrar los totales generales para las columnas de esta PivotTable. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Indica si se deben mostrar descripciones emergentes para las celdas de datos de PivotTable. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Establece si se muestran los botones de expandir/contraer. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Indica si se deben incluir columnas vacías en la tabla |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Indica si se deben incluir filas vacías en la tabla. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Indica si se deben mostrar los títulos de los campos de datos y los títulos de los campos de pivote en el eje de filas y el eje de columnas en la vista de PivotTable. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Especifica un valor booleano que indica si la información de propiedades de miembros debe omitirse de las descripciones emergentes de PivotTable. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Indica si el encabezado de columna en la PivotTable debe tener aplicado el estilo. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Indica si se aplica formato de franjas a la columna. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Indica si se aplica el formato de columna. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Indica si el encabezado de fila en la PivotTable debe tener aplicado el estilo. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Indica si se aplica formato de franjas a las filas. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Indica si se deben mostrar los totales generales para las filas de la PivotTable. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Indica si el título del encabezado de fila se muestra en el informe de PivotTable Indica si se muestran los títulos de los campos de visualización y los menús desplegables de filtro |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Indica si se muestra la fila de valores. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Indica si los elementos de campo de página ocultos en el informe de PivotTable se incluyen en los subtotales de filas y columnas, totales de bloque y totales generales. |
| [setTag(String value)](#setTag-java.lang.String-) | Establece una cadena definida por el usuario que está asociada a esta vista de tabla dinámica. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Mostrar el detalle de un elemento en la región de datos en una nueva tabla. |
| [showInCompactForm()](#showInCompactForm--) | Diseña la vista de PivotTable en forma compacta. |
| [showInOutlineForm()](#showInOutlineForm--) | Diseña el PivotTable en forma de esquema. |
| [showInTabularForm()](#showInTabularForm--) | Diseña el PivotTable en forma tabular. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Mostrar todas las páginas de filtro de informe según PivotField, el PivotField debe estar ubicado en PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Mostrar todas las páginas de filtro de informe según el índice de posición en PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Mostrar todas las páginas de filtro de informe según el nombre de PivotField, el PivotField debe estar ubicado en PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Agrega un campo calculado al campo dinámico y lo arrastra al área de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del campo calculado |
| formula | java.lang.String | La fórmula del campo calculado. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Agrega un campo calculado al campo dinámico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del campo calculado |
| formula | java.lang.String | La fórmula del campo calculado. |
| dragToDataArea | boolean | True, arrastre este campo al área de datos inmediatamente |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Agrega el campo al área específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). el tipo de área de campos. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | el campo en los campos base. |

**Returns:**
int - la posición del campo en los campos específicos.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Agrega el campo al área específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de área de campos. |
| baseFieldIndex | int | El índice en los campos base. |

**Returns:**
int - La posición del campo en los campos específicos.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Agrega el campo al área específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de área de campos. |
| fieldName | java.lang.String | El nombre en los campos base. |

**Returns:**
int - La posición del campo en los campos específicos. Si no existe un campo con ese nombre, devolver -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcula los datos de la tabla dinámica a celdas.

**Remarks**

Este método solo calcula datos con la caché en [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Por lo tanto, si desea calcular con la fuente de datos más reciente, utilice el método [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) para calcular. Si solo se cambió la configuración de la tabla dinámica, [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) es suficiente.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Calcula la tabla dinámica con opciones.

**Remarks**

Si [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) es true, este método actualizará la caché de la tabla dinámica desde la fuente de datos, luego calculará todas las tablas dinámicas basadas en la misma caché. De lo contrario, solo se calculará con los datos en caché en la caché de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Las opciones para calcular la tabla dinámica |

**Returns:**
com.aspose.cells.PivotTable[] - Devuelve todas las tablas dinámicas que han sido calculadas. Si [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) es true, todas las tablas dinámicas basadas en la misma caché se calcularán juntas.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Calcula el rango de la tabla dinámica.

**Remarks**

Si este método no ha sido llamado, tal vez el rango de la tabla dinámica no esté correcto.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Cambiar la fuente de datos de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Eliminar todos los campos de las regiones.

### clearData() {#clearData--}
```
public void clearData()
```


Borrar datos y formato de la vista de la tabla dinámica.

**Remarks**

Si este método no se llama antes de agregar o eliminar PivotField, es posible que los datos de la PivotTable no estén correctos

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Borra todos los filtros de esta tabla dinámica.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Copia el estilo con nombre de otra tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Tabla dinámica de origen. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Exporta la vista de tabla dinámica como JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Obtiene los campos específicos por el tipo de campo.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.GetFields(PivotFieldType). Este método será eliminado 12 meses después, a partir de mayo de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). el tipo de campo. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Da formato al área seleccionada de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango de las celdas. |
| style | [Style](../../com.aspose.cells/style) | El estilo |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Da formato al área seleccionada de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | El área de vista de pivote seleccionada. |
| style | [Style](../../com.aspose.cells/style) | La configuración formateada. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Da formato a la celda en el área de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila de la celda |
| columna | int | Índice de columna de la celda |
| style | [Style](../../com.aspose.cells/style) | Estilo que se utiliza para formatear la celda |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Da formato a todas las celdas en el área de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Estilo que se utiliza para formatear |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Da formato a los datos de fila en el área de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila del objeto Row |
| style | [Style](../../com.aspose.cells/style) | Estilo que se utiliza para formatear |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Obtiene la descripción del texto alternativo.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Obtiene el título del texto alternativo.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Obtiene el tipo de formato automático de la tabla dinámica.

Ver [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Indica si ajustar automáticamente el ancho de columna al actualizar.

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Devuelve todos los campos base de la tabla dinámica.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Obtiene el área que contiene el botón de campo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de región. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Obtiene el objeto [Cell](../../com.aspose.cells/cell) por el nombre para mostrar del PivotField.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| displayName | java.lang.String | el DisplayName de PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Obtiene las tablas dinámicas hijas que utilizan los datos de esta tabla dinámica como fuente de datos.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.GetDependentPivotTables(). Este método será eliminado 12 meses después, a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
com.aspose.cells.PivotTable[] - el objeto array de PivotTable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Devuelve un objeto PivotFields que se muestra actualmente como campos de columna.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Indica si el informe de tabla dinámica muestra totales generales para las columnas.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.ShowColumnGrandTotals. Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Obtiene el título personalizado del encabezado de columna de la tabla dinámica.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Devuelve un objeto CellArea que representa el rango que contiene el área de columna en el informe de PivotTable. Solo lectura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Obtiene los formatos condicionales de la tabla dinámica.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Indica si se considera la lista personalizada incorporada al ordenar datos.

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Devuelve un objeto [CellArea](../../com.aspose.cells/cellarea) que representa el rango que contiene el área de datos en la lista entre la fila de encabezado y la fila de inserción. Solo lectura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Obtiene un objeto [PivotField](../../com.aspose.cells/pivotfield) que representa todos los campos de datos en una PivotTable. Solo lectura. Solo se creará cuando haya dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puede arrastrarlo a la región de filas/columnas con el método PivotTable.AddFieldToArea().

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotTable.ValuesField. Este método será eliminado 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Obtiene el nombre del encabezado del campo del área de valores en la tabla dinámica.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Obtiene una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que representa todos los campos de datos en una tabla dinámica.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Obtiene la fuente de datos de la tabla dinámica.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Obtiene todas las [PivotTable](../../com.aspose.cells/pivottable)s que usan esta tabla dinámica como su fuente de datos.

**Remarks**

Debido a que las tablas dinámicas pueden depender de los datos de otras, deben actualizarse en el orden correcto para garantizar la consistencia de los datos.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Indica si el informe de la tabla dinámica muestra una cadena personalizada en celdas que contienen errores.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la PivotTable está vacía. El valor predeterminado es true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Indica si el informe de la tabla dinámica muestra una cadena personalizada si el valor es nulo.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Especifica un valor booleano que indica si al usuario se le permite editar las celdas en el área de datos de la PivotTable. El valor predeterminado es false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Indica si la perforación (drilldown) está habilitada.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Indica si el cuadro de diálogo de campo de tabla dinámica está disponible cuando el usuario hace doble clic en el campo de la tabla dinámica.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Indica si la lista de campos para la tabla dinámica está disponible en la vista de Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Indica si el Asistente de tabla dinámica está disponible.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Obtiene la cadena mostrada en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Obtiene la fuente de datos de la conexión externa.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.GetSourceDataConnections(). Este método será eliminado 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Indica si los campos en la tabla dinámica están ordenados en un orden no predeterminado en la lista de campos.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Obtiene la lista de campos de tabla dinámica específica por la región.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). el tipo de región. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Obtiene el área de la región de filtro.

**Remarks**

Solo es válido si existen campos de filtro de tabla dinámica. Se devolverá un área vacía si esta tabla dinámica no contiene campos de filtro.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Devuelve la etiqueta que se muestra en el encabezado de la columna o fila del total general. El valor predeterminado es la cadena "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Obtiene la lista de índices de fila de la tabla dinámica de saltos de página horizontales

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.GetHorizontalPageBreaks(). Este método será eliminado 12 meses después a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Obtiene los saltos de página horizontales de esta tabla dinámica.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en Forma Compacta.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.RepeatItemsOnEachPrintedPage. Este método será eliminado 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Indica si el informe de la tabla dinámica se recalcula solo a solicitud del usuario.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Obtiene si se deben combinar las etiquetas de campo de fila/columna que abarcan varias celdas.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

Ver [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotCache.MissingItemsLimit. Este método será eliminado 12 meses después a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la tabla dinámica

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Obtiene los nombres de las conexiones de datos de origen externo.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Obtiene la cadena mostrada en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Obtiene el orden en que los campos de página se añaden al diseño del informe de tabla dinámica.

Ver [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Obtiene el número de campos de página en cada columna o fila del informe de tabla dinámica.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Devuelve una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que se muestra actualmente como campos de página.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Obtiene la fuente de datos.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Devuelve todos los filtros en la tabla dinámica.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Obtiene las condiciones de formato de la tabla dinámica.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.ConditionalFormats. Este método será eliminado 12 meses después a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Obtiene todos los formatos de celda aplicados a esta tabla dinámica.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Obtiene la configuración de [TableStyle](../../com.aspose.cells/tablestyle) de esta tabla dinámica.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Obtiene el nombre del estilo de la tabla dinámica.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Obtiene el estilo incorporado de la tabla dinámica.

Ver [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Obtiene todas las tablas dinámicas con la misma caché de tabla dinámica.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Indica si se debe preservar el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) cuando la tabla dinámica se actualiza o recalcula.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Indica si el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) se preserva cuando la tabla dinámica se actualiza o recalcula.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.PreserveCellFormattingOnUpdate. Este método será eliminado 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Especifica un valor booleano que indica si los indicadores de perforación deben imprimirse. Imprime los botones de expandir/contraer cuando se muestran en la PivotTable.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de la PivotTable. El valor predeterminado es false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Indica si se deben actualizar los datos al abrir el archivo.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Obtiene la fecha y hora de la última actualización de la tabla dinámica.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Obtiene el nombre del último usuario que actualizó esta tabla dinámica

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Devuelve una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) que se muestra actualmente como campos de fila.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Indica si se deben mostrar los totales generales para las filas de esta tabla dinámica.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.ShowRowGrandTotals. Este método será eliminado 12 meses después a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Obtiene el título personalizado del encabezado de fila en esta tabla dinámica.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Devuelve un objeto CellArea que representa el rango que contiene el área de fila en el informe de la PivotTable. Solo lectura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Indica si los datos del informe de PivotTable se guardan con el libro.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Indica si se deben mostrar los totales generales para las columnas de esta PivotTable.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Indica si se deben mostrar descripciones emergentes para las celdas de datos de PivotTable.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Obtiene si se muestran los botones de expandir/contraer.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Indica si se deben incluir columnas vacías en la tabla

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Indica si se deben incluir filas vacías en la tabla.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Indica si se deben mostrar los títulos de los campos de datos y los títulos de los campos de pivote en el eje de filas y el eje de columnas en la vista de PivotTable.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Especifica un valor booleano que indica si la información de propiedades de miembros debe omitirse de las descripciones emergentes de PivotTable.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Indica si el encabezado de columna en la PivotTable debe tener aplicado el estilo.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Indica si se aplica formato de franjas a la columna.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Indica si se aplica el formato de columna.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Indica si el encabezado de fila en la PivotTable debe tener aplicado el estilo.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Indica si se aplica formato de franjas a las filas.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Indica si se deben mostrar los totales generales para las filas de la PivotTable.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Indica si el título del encabezado de fila se muestra en el informe de PivotTable Indica si se muestran los títulos de los campos de visualización y los menús desplegables de filtro

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.ShowHeaders. Este método será eliminado 12 meses después a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Indica si se muestra la fila de valores.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Obtén la fuente de datos de esta PivotTable.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Obtén la fuente de datos de esta PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isOriginal | boolean | Indica si se debe devolver el origen original o el origen de datos de visualización. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Obtiene las fuentes de datos de conexión externa.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Obtiene el tipo de fuente de datos de la PivotTable.

Ver [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Indica si los elementos de campo de página ocultos en el informe de la PivotTable se incluyen en los subtotales de fila y columna, totales de bloque y totales generales. El valor predeterminado es False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Devuelve un objeto CellArea que representa el rango que contiene todo el informe de PivotTable, pero no incluye los campos de página. Solo lectura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Devuelve un objeto CellArea que representa el rango que contiene todo el informe de PivotTable, incluye los campos de página. Solo lectura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Obtiene una cadena definida por el usuario que está asociada con esta vista de PivotTable.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Representa el área en blanco en la esquina superior derecha de la PivotTable (esquina superior izquierda para hojas RTL).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Obtiene un objeto [PivotField](../../com.aspose.cells/pivotfield) que representa todos los campos de datos en una PivotTable. Solo lectura. Solo se creará cuando haya dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puede arrastrarlo a la región de filas/columnas con el método PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de PivotTable que requieren agregar filas en blanco.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice la propiedad PivotField.InsertBlankRow. Este método será eliminado 12 meses después, a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Indica si el informe de PivotTable se formatea automáticamente. Casilla de verificación \"autoformat table\" que está en la opción de pivottable para Excel 2003.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Especifica si la PivotTable es compatible con Excel2003 al actualizarla; si es verdadero, una cadena debe tener 255 caracteres o menos, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, la cadena no tendrá la restricción mencionada. El valor predeterminado es verdadero.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Indica si el informe de PivotTable muestra el diseño clásico de pivottable. (permite arrastrar campos en la cuadrícula)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice la propiedad PivotTable.AllowMultipleFiltersPerField. Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indica si esta tabla dinámica está seleccionada.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice el método PivotTable.MoveTo(). Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | índice de fila. |
| columna | int | índice de columna. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice el método PivotTable.MoveTo(). Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destCellName | java.lang.String | el nombre de la celda de destino. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Mueve un elemento hacia arriba o hacia abajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La región. Solo para fila o columna. |
| nodos | java.lang.String[] | El elemento. |
| absoluto | boolean | Indica si el desplazamiento es una posición absoluta. |
| desplazamiento | int | Si absoluto es verdadero: 0 mueve al inicio, -1 mueve al final, los demás indican posición absoluta; de lo contrario, desplazamiento es una posición relativa. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | índice de fila. |
| columna | int | índice de columna. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | el índice de la hoja de cálculo objetivo |
| fila | int | índice de fila. |
| columna | int | índice de columna. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destCellName | java.lang.String | el nombre de la celda de destino. |

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
public int refresh()
```


Actualiza [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica.

**Remarks**

Todas las tablas dinámicas que dependen del mismo PivotCache se recalcularán.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Actualiza [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica.

**Remarks**

Todas las tablas dinámicas que dependen del mismo PivotCache se recalcularán.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Actualiza los datos desde su fuente de datos al caché de tabla dinámica.

**Remarks**

Recopilaremos datos de la fuente de datos a un pivot cache, luego calcularemos los datos en el caché en las celdas. Y es mejor que simplemente llame a [Workbook.refreshAll()](../../com.aspose.cells/workbook\\#refreshAll--) para actualizar y calcular todas las tablas dinámicas en el archivo, en lugar de actualizarlas una por una. NOTA: Este método está obsoleto. En su lugar, utilice el método [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) y elimine el siguiente [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) porque esta tabla dinámica se calculará al actualizar [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--). Este método será eliminado 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos con opciones.

**Remarks**

Recopilaremos datos de la fuente de datos a un pivot cache, luego calcularemos los datos en el caché en las celdas. Y es mejor que simplemente llame a [Workbook.refreshAll()](../../com.aspose.cells/workbook\\#refreshAll--) para actualizar y calcular todas las tablas dinámicas en el archivo, en lugar de actualizarlas una por una. NOTA: Este método está obsoleto. En su lugar, utilice el método [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) y elimine el siguiente [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) porque esta tabla dinámica se calculará al actualizar [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--). Este método será eliminado 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Las opciones para actualizar la fuente de datos de la tabla dinámica. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Eliminar campo del área de campo específica

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). el tipo de área de campos. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | el campo en los campos base. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Elimina un campo de una región de tabla dinámica específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de área de campos. |
| baseFieldIndex | int | El índice de campo en los campos base. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Elimina un campo del área de campo específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de área de campos. |
| fieldName | java.lang.String | El nombre en los campos base. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Selecciona un área de la vista de tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El área de la celda. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Obtiene la descripción del texto alternativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Establece el título del texto alternativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Indica si el informe de PivotTable se formatea automáticamente. Casilla de verificación \"autoformat table\" que está en la opción de pivottable para Excel 2003.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Establece el tipo de formato automático de la tabla dinámica.

Ver [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Indica si ajustar automáticamente el ancho de columna al actualizar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Indica si el informe de tabla dinámica muestra totales generales para las columnas.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.ShowColumnGrandTotals. Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Establece el título personalizado del encabezado de columna de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Indica si se considera la lista personalizada incorporada al ordenar datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Establece el nombre del encabezado del campo del área de valores en la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Establece la fuente de datos de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Indica si el informe de la tabla dinámica muestra una cadena personalizada en celdas que contienen errores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la PivotTable está vacía. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Indica si el informe de la tabla dinámica muestra una cadena personalizada si el valor es nulo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Especifica un valor booleano que indica si al usuario se le permite editar las celdas en el área de datos de la PivotTable. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Indica si la perforación (drilldown) está habilitada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Indica si el cuadro de diálogo de campo de tabla dinámica está disponible cuando el usuario hace doble clic en el campo de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Indica si la lista de campos para la tabla dinámica está disponible en la vista de Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Indica si el Asistente de tabla dinámica está disponible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Obtiene la cadena mostrada en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Especifica si la PivotTable es compatible con Excel2003 al actualizarla; si es verdadero, una cadena debe tener 255 caracteres o menos, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, la cadena no tendrá la restricción mencionada. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Indica si los campos en la tabla dinámica están ordenados en un orden no predeterminado en la lista de campos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Devuelve la etiqueta que se muestra en el encabezado de la columna o fila del total general. El valor predeterminado es la cadena "Grand Total".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Indica si el informe de PivotTable muestra el diseño clásico de pivottable. (permite arrastrar campos en la cuadrícula)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de PivotTable que requieren agregar filas en blanco.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice la propiedad PivotField.InsertBlankRow. Este método será eliminado 12 meses después, a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en Forma Compacta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.RepeatItemsOnEachPrintedPage. Este método será eliminado 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Indica si el informe de la tabla dinámica se recalcula solo a solicitud del usuario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Establece si se deben combinar las etiquetas de campo de fila/columna que abarcan varias celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

Ver [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotCache.MissingItemsLimit. Este método será eliminado 12 meses después a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros aplicados.

**Remarks**

NOTA: Esta propiedad está obsoleta. En su lugar, utilice la propiedad PivotTable.AllowMultipleFiltersPerField. Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtiene el nombre de la tabla dinámica

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Obtiene la cadena mostrada en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Establece el orden en que los campos de página se añaden al diseño del informe de tabla dinámica.

Ver [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Obtiene el número de campos de página en cada columna o fila del informe de tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Obtiene la configuración de [TableStyle](../../com.aspose.cells/tablestyle) de esta tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Establece el nombre del estilo de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Establece el estilo incorporado de la tabla dinámica.

Ver [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Indica si se debe preservar el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) cuando la tabla dinámica se actualiza o recalcula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Indica si el formato de celda ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) se preserva cuando la tabla dinámica se actualiza o recalcula.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.PreserveCellFormattingOnUpdate. Este método será eliminado 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Especifica un valor booleano que indica si los indicadores de perforación deben imprimirse. Imprime los botones de expandir/contraer cuando se muestran en la PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de la PivotTable. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Indica si se deben actualizar los datos al abrir el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Indica si se deben mostrar los totales generales para las filas de esta tabla dinámica.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.ShowRowGrandTotals. Este método será eliminado 12 meses después a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Establece el título personalizado del encabezado de fila en esta tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Indica si los datos del informe de PivotTable se guardan con el libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica si esta tabla dinámica está seleccionada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Indica si se deben mostrar los totales generales para las columnas de esta PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Indica si se deben mostrar descripciones emergentes para las celdas de datos de PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Establece si se muestran los botones de expandir/contraer.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Indica si se deben incluir columnas vacías en la tabla

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Indica si se deben incluir filas vacías en la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Indica si se deben mostrar los títulos de los campos de datos y los títulos de los campos de pivote en el eje de filas y el eje de columnas en la vista de PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Especifica un valor booleano que indica si la información de propiedades de miembros debe omitirse de las descripciones emergentes de PivotTable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Indica si el encabezado de columna en la PivotTable debe tener aplicado el estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Indica si se aplica formato de franjas a la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Indica si se aplica el formato de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Indica si el encabezado de fila en la PivotTable debe tener aplicado el estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Indica si se aplica formato de franjas a las filas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Indica si se deben mostrar los totales generales para las filas de la PivotTable.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Indica si el título del encabezado de fila se muestra en el informe de PivotTable Indica si se muestran los títulos de los campos de visualización y los menús desplegables de filtro

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.ShowHeaders. Este método será eliminado 12 meses después a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Indica si se muestra la fila de valores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Indica si los elementos de campo de página ocultos en el informe de la PivotTable se incluyen en los subtotales de fila y columna, totales de bloque y totales generales. El valor predeterminado es False.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Establece una cadena definida por el usuario que está asociada a esta vista de tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Mostrar el detalle de un elemento en la región de datos en una nueva tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | Desplazamiento a la primera fila de datos en la región de datos. |
| columnOffset | int | Desplazamiento a la primera columna de datos en la región de datos. |
| newSheet | boolean | Mostrar el detalle en una nueva hoja de cálculo. |
| destRow | int | La fila de destino. |
| destColumn | int | La columna de destino. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Diseña la vista de PivotTable en forma compacta.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Diseña el PivotTable en forma de esquema.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Diseña el PivotTable en forma tabular.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Mostrar todas las páginas de filtro de informe según PivotField, el PivotField debe estar ubicado en PageFields.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | El objeto PivotField |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Mostrar todas las páginas de filtro de informe según el índice de posición en PageFields.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| posIndex | int | El índice de posición en los PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Mostrar todas las páginas de filtro de informe según el nombre de PivotField, el PivotField debe estar ubicado en PageFields.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | java.lang.String | El nombre de PivotField |

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

