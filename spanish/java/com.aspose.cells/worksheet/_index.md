---
title: "Worksheet"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una sola hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Encapsula el objeto que representa una sola hoja de cálculo.

**Example**

El siguiente ejemplo muestra cómo congelar paneles e insertar un hipervínculo en la hoja de cálculo con .Net o VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Agrega salto de página. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filtra datos usando criterios complejos. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajusta automáticamente el ancho de la columna. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Ajusta automáticamente el ancho de la columna. |
| [autoFitColumns()](#autoFitColumns--) | Ajusta automáticamente todas las columnas en esta hoja de cálculo. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente todas las columnas en esta hoja de cálculo. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Ajusta automáticamente el ancho de las columnas. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente el ancho de las columnas. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Ajusta automáticamente el ancho de las columnas. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente el ancho de las columnas. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Ajusta automáticamente la altura de la fila. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Ajusta automáticamente la altura de la fila. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente la altura de la fila. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Ajusta automáticamente la altura de la fila en un rango rectangular. |
| [autoFitRows()](#autoFitRows--) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Ajusta automáticamente la altura de la fila en un rango. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Ajusta automáticamente la altura de la fila en un rango. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcula una fórmula como fórmula de matriz. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Calcula una fórmula como fórmula de matriz. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Calcula una fórmula como fórmula de matriz. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Calcula todas las fórmulas en esta hoja de cálculo. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcula una fórmula. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcula directamente una expresión de fórmula. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Calcula directamente una expresión de fórmula. |
| [clearComments()](#clearComments--) | Elimina todos los comentarios en la hoja de cálculo del diseñador. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Cierra la sesión que usa cachés para acceder a los datos en esta hoja de cálculo. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Convierte el estilo de referencia de la fórmula. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Copia el contenido y los formatos de otra hoja de cálculo. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Copia el contenido y los formatos de otra hoja de cálculo. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Filtra el rango. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [getActiveCell()](#getActiveCell--) | Obtiene la celda activa en la hoja de cálculo. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Obtiene la configuración del filtro avanzado. |
| [getAllPictures()](#getAllPictures--) | Obtiene todas las imágenes, incluidas las que están incrustadas en la celda y sobre las celdas. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Obtiene la colección de rangos de edición permitida en la hoja de cálculo. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Consulta áreas de celdas que están mapeadas/vinculadas a la ruta específica del mapa XML. |
| [getAutoFilter()](#getAutoFilter--) | Representa el filtro automático para la hoja de cálculo especificada. |
| [getBackgroundImage()](#getBackgroundImage--) | Obtiene la imagen de fondo de la hoja de cálculo. |
| [getCellWatches()](#getCellWatches--) | Obtiene la colección de celdas en esta hoja de cálculo que se están observando en la 'ventana de observación'. |
| [getCells()](#getCells--) | Obtiene la colección de [Cells](../../com.aspose.cells/cells). |
| [getCharts()](#getCharts--) | Obtiene una colección de [Chart](../../com.aspose.cells/chart) |
| [getCheckBoxes()](#getCheckBoxes--) | Obtiene una colección de [CheckBox](../../com.aspose.cells/checkbox). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Obtiene el nombre de código de la hoja de cálculo. |
| [getComments()](#getComments--) | Obtiene la colección de [Comment](../../com.aspose.cells/comment). |
| [getConditionalFormattings()](#getConditionalFormattings--) | Obtiene los ConditionalFormattings en la hoja de cálculo. |
| [getCustomProperties()](#getCustomProperties--) | Obtiene un objeto que representa la información de identificador asociada a una hoja de cálculo. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. |
| [getDisplayZeros()](#getDisplayZeros--) | Verdadero si se muestran valores cero. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Obtiene la configuración de verificación de errores aplicada a ciertos rangos. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Representa el índice de la primera columna visible. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Representa el índice de la primera fila visible. |
| [getFreezedPanes()](#getFreezedPanes--) | Obtiene los paneles congelados. |
| [getGridlineColor()](#getGridlineColor--) | Obtiene el color de la línea de cuadrícula |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Obtiene la colección de [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection). |
| [getHyperlinks()](#getHyperlinks--) | Obtiene la colección de [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection). |
| [getIndex()](#getIndex--) | Obtiene el índice de la hoja en la colección de hojas de cálculo. |
| [getListObjects()](#getListObjects--) | Obtiene todos los ListObjects en esta hoja de cálculo. |
| [getName()](#getName--) | Obtiene el nombre de la hoja de cálculo. |
| [getOleObjects()](#getOleObjects--) | Representa una colección de [OleObject](../../com.aspose.cells/oleobject) en una hoja de cálculo. |
| [getOutline()](#getOutline--) | Obtiene el contorno en esta hoja de cálculo. |
| [getPageSetup()](#getPageSetup--) | Representa la descripción de la configuración de página en esta hoja. |
| [getPaneState()](#getPaneState--) | Indica si el panel tiene divisiones horizontales o verticales, y si esas divisiones están congeladas. |
| [getPanes()](#getPanes--) | Obtiene los paneles de ventana. |
| [getPictures()](#getPictures--) | Obtiene una colección de [Picture](../../com.aspose.cells/picture). |
| [getPivotTables()](#getPivotTables--) | Obtiene todas las tablas dinámicas en esta hoja de cálculo. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Obtiene saltos de página automáticos. |
| [getProtection()](#getProtection--) | Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo. |
| [getQueryTables()](#getQueryTables--) | Obtiene [QueryTableCollection](../../com.aspose.cells/querytablecollection) en la hoja de cálculo. |
| [getScenarios()](#getScenarios--) | Obtiene la colección de [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador. |
| [getSelectedRanges()](#getSelectedRanges--) | Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador. |
| [getShapes()](#getShapes--) | Devuelve todas las formas de dibujo en esta hoja de cálculo. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Indica si se deben mostrar los íconos de tipo de datos. |
| [getShowFormulas()](#getShowFormulas--) | Indica si se deben mostrar las fórmulas o sus resultados. |
| [getSlicers()](#getSlicers--) | Obtiene la colección de Slicer en la hoja de cálculo |
| [getSmartTagSetting()](#getSmartTagSetting--) | Obtiene todos los objetos de [SmartTagCollection](../../com.aspose.cells/smarttagcollection) de la hoja de cálculo. |
| [getSparklineGroups()](#getSparklineGroups--) | Obtiene los grupos de sparkline en la hoja de cálculo. |
| [getTabColor()](#getTabColor--) | Representa el color de la pestaña de la hoja de cálculo. |
| [getTabId()](#getTabId--) | Especifica el identificador interno de la hoja. |
| [getTextBoxes()](#getTextBoxes--) | Obtiene una colección de [TextBox](../../com.aspose.cells/textbox). |
| [getTimelines()](#getTimelines--) | Obtiene la colección de Timeline en la hoja de cálculo |
| [getTransitionEntry()](#getTransitionEntry--) | Indica si la opción de Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Indica si la opción de Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [getType()](#getType--) | Representa el tipo de hoja de cálculo. |
| [getUniqueId()](#getUniqueId--) | Obtiene el id único, es el mismo que \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Obtiene la colección de [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection). |
| [getViewType()](#getViewType--) | Obtiene el tipo de vista. |
| [getVisibilityType()](#getVisibilityType--) | Indica el estado visible de esta hoja. |
| [getWorkbook()](#getWorkbook--) | Obtiene el objeto del libro de trabajo que contiene esta hoja. |
| [getZoom()](#getZoom--) | Representa el factor de escala en porcentaje. |
| [hasAutofilter()](#hasAutofilter--) | Indica si esta hoja de cálculo tiene filtro automático. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Obtiene un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero. |
| [isOutlineShown()](#isOutlineShown--) | Indica si se muestra el contorno. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página. |
| [isProtected()](#isProtected--) | Indica si la hoja de cálculo está protegida. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Obtiene un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. |
| [isRulerVisible()](#isRulerVisible--) | Indica si la regla es visible. |
| [isSelected()](#isSelected--) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro. |
| [isVisible()](#isVisible--) | Representa si la hoja de cálculo es visible. |
| [moveTo(int index)](#moveTo-int-) | Mueve la hoja a otra ubicación en la hoja de cálculo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Protege la hoja de cálculo. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Protege la hoja de cálculo. |
| [refreshPivotTables()](#refreshPivotTables--) | Actualiza todas las tablas dinámicas en esta hoja de cálculo. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Actualiza todas las tablas dinámicas en esta hoja de cálculo. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Elimina todos los objetos de dibujo en esta hoja de cálculo. |
| [removeAutoFilter()](#removeAutoFilter--) | Elimina el filtro automático de la hoja de cálculo. |
| [removeSplit()](#removeSplit--) | Elimina la ventana dividida. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Reemplaza el texto de todas las celdas con una nueva cadena. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Selecciona un rango. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Establece la celda activa en la hoja de cálculo. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Establece la imagen de fondo de la hoja de cálculo. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Obtiene el nombre de código de la hoja de cálculo. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Verdadero si se muestran valores cero. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Representa el índice de la primera columna visible. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Representa el índice de la primera fila visible. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Establece el color de la línea de cuadrícula |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la hoja de cálculo. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indica si se muestra el contorno. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Establece un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Indica si la regla es visible. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Indica si se deben mostrar los íconos de tipo de datos. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Indica si se deben mostrar las fórmulas o sus resultados. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Representa el color de la pestaña de la hoja de cálculo. |
| [setTabId(int value)](#setTabId-int-) | Especifica el identificador interno de la hoja. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Indica si la opción de Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Indica si la opción de Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada. |
| [setType(int value)](#setType-int-) | Representa el tipo de hoja de cálculo. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Establece el id único, es el mismo que \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Establece el tipo de vista. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Indica el estado visible de esta hoja. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representa si la hoja de cálculo es visible. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Establece las opciones visibles. |
| [setZoom(int value)](#setZoom-int-) | Representa el factor de escala en porcentaje. |
| [split()](#split--) | Divide la ventana. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Inicia la sesión que usa cachés para acceder a los datos en esta hoja de cálculo. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Worksheet actual. |
| [unFreezePanes()](#unFreezePanes--) | Descongela los paneles en la hoja de cálculo. |
| [unprotect()](#unprotect--) | Desprotege la hoja de cálculo. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Desprotege la hoja de cálculo. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Consulta áreas de celdas que están mapeadas/vinculadas a la ruta específica del mapa XML. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Agrega salto de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filtra datos usando criterios complejos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFilter | boolean | Indica si se filtra la lista en el lugar. |
| listRange | java.lang.String | El rango de la lista. |
| criteriaRange | java.lang.String | El rango de criterios. |
| copyTo | java.lang.String | El rango al que se copian los datos. |
| uniqueRecordOnly | boolean | Solo muestra o copia filas únicas. |

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


Ajusta automáticamente todas las columnas en esta hoja de cálculo.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Ajusta automáticamente todas las columnas en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones de ajuste automático |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Ajusta automáticamente el ancho de las columnas.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstColumn | int | Índice de la primera columna. |
| lastColumn | int | Último índice de columna. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Ajusta automáticamente el ancho de las columnas.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstColumn | int | Índice de la primera columna. |
| lastColumn | int | Último índice de columna. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones de ajuste automático |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Ajusta automáticamente el ancho de las columnas.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Índice de la primera fila. |
| firstColumn | int | Índice de la primera columna. |
| lastRow | int | Índice de la última fila. |
| lastColumn | int | Último índice de columna. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Ajusta automáticamente el ancho de las columnas.

**Remarks**

AutoFitColumn es una función imprecisa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Índice de la primera fila. |
| firstColumn | int | Índice de la primera columna. |
| lastRow | int | Índice de la última fila. |
| lastColumn | int | Último índice de columna. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones de ajuste automático |

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

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
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
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones del ajuste automático |

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

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Ajusta automáticamente todas las filas en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones del ajuste automático |

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

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Ajusta automáticamente la altura de la fila en un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Las opciones del ajuste automático. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Calcula una fórmula como fórmula de matriz.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones para calcular la fórmula |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Calcula una fórmula como fórmula de matriz.

**Remarks**

La fórmula se tomará como una fórmula de matriz dinámica para calcular la dimensión y el resultado. La dimensión máxima especificada por el usuario se utiliza en casos en que el resultado calculado es un conjunto de datos grande (por ejemplo, el resultado calculado puede corresponder a una fila o columna completa) pero el usuario no necesita una matriz tan grande según los requisitos del negocio o por consideraciones de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones para calcular la fórmula |
| maxRowCount | int | el número máximo de filas de los datos resultantes. Si es no positivo o mayor que el número real de filas, se utilizará el número real de filas. |
| maxColumnCount | int | el número máximo de columnas de los datos resultantes. Si es no positivo o mayor que el número real de filas, se utilizará el número real de columnas. |

**Returns:**
java.lang.Object[][] - Resultado de la fórmula calculada.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Calcula una fórmula como fórmula de matriz.

**Remarks**

La fórmula se tomará como una fórmula de matriz dinámica para calcular la dimensión y el resultado. La dimensión máxima especificada por el usuario se utiliza en casos en que el resultado calculado es un conjunto de datos grande (por ejemplo, el resultado calculado puede corresponder a una fila o columna completa) pero el usuario no necesita una matriz tan grande según los requisitos del negocio o por consideraciones de rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones para calcular la fórmula |
| baseCellRow | int | El índice de fila de la celda base. |
| baseCellColumn | int | El índice de columna de la celda base. |
| maxRowCount | int | El número máximo de filas de los datos resultantes. Si es no positivo o mayor que el número real de filas, se utilizará el número real de filas. |
| maxColumnCount | int | El número máximo de columnas de los datos resultantes. Si es no positivo o mayor que el recuento real de filas, se usará el recuento real de columnas. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Los datos de cálculo. Se utilizan para la situación en que el usuario necesita calcular algunas fórmulas estáticas al implementar un motor de cálculo personalizado. Para este tipo de situación, el usuario debe especificarlos con los datos de cálculo proporcionados para [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - Resultado de la fórmula calculada.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Calcula todas las fórmulas en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones de cálculo |
| recursive | boolean | True indica que si las celdas de la hoja dependen de celdas de otras hojas, las celdas dependientes en otras hojas también se calcularán. False indica que todas las fórmulas en la hoja se han calculado y los valores son correctos. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcula una fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |

**Returns:**
java.lang.Object - Resultado de la fórmula calculada.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Calcula directamente una expresión de fórmula.

**Remarks**

La fórmula se calculará como si se hubiera establecido en la celda A1. Y la fórmula se tomará como una fórmula normal. Si necesita que la fórmula se calcule como una fórmula de matriz y obtener una matriz para el resultado calculado, utilice [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) en su lugar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones para calcular la fórmula |

**Returns:**
java.lang.Object - Resultado calculado de la fórmula dada. El objeto devuelto puede ser de los tipos posibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Calcula directamente una expresión de fórmula.

**Remarks**

La fórmula se calculará como si se hubiera establecido en la celda base especificada. Y la fórmula se tomará como una fórmula normal. Si necesita que la fórmula se calcule como una fórmula de matriz y obtener una matriz para el resultado calculado, utilice [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) en su lugar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | Fórmula a calcular. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones para calcular la fórmula. |
| baseCellRow | int | El índice de fila de la celda base. |
| baseCellColumn | int | El índice de columna de la celda base. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Los datos de cálculo. Se utilizan para la situación en que el usuario necesita calcular algunas fórmulas estáticas al implementar un motor de cálculo personalizado. Para este tipo de situación, el usuario debe especificarlos con los datos de cálculo proporcionados para [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - Resultado calculado de la fórmula dada. El objeto devuelto puede ser de los tipos posibles de [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Elimina todos los comentarios en la hoja de cálculo del diseñador.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Cierra la sesión que usa cachés para acceder a los datos en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opciones de acceso a datos |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Convierte el estilo de referencia de la fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula a convertir. |
| toR1C1 | boolean | Qué estilo de referencia convertir la fórmula. Si la fórmula original está en estilo de referencia A1, este valor debe ser true para que la fórmula se convierta de A1 a estilo de referencia R1C1; si la fórmula original está en estilo de referencia R1C1, este valor debe ser false para que la fórmula se convierta de R1C1 a estilo A1; |
| baseCellRow | int | El índice de fila de la celda base. |
| baseCellColumn | int | El índice de columna de la celda base. |

**Returns:**
java.lang.String - La fórmula convertida.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Copia el contenido y los formatos de otra hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Hoja de origen. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Copia el contenido y los formatos de otra hoja de cálculo.

**Remarks**

Puede copiar datos de otra hoja en el mismo archivo o en otro archivo. Sin embargo, este método no admite copiar objetos de dibujo, como comentarios, imágenes y gráficos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Hoja de origen. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Filtra el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango |

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
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Obtiene la configuración del filtro avanzado.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Obtiene todas las imágenes, incluidas las que están incrustadas en la celda y sobre las celdas.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Obtiene la colección de rangos de edición permitida en la hoja de cálculo.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Consulta áreas de celdas que están mapeadas/vinculadas a la ruta específica del mapa XML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | ruta del elemento xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Especifique un mapa xml si desea consultar la ruta específica dentro de un mapa específico |

**Returns:**
com.aspose.cells.CellArea[] - lista de [CellArea](../../com.aspose.cells/cellarea) que está mapeada/vinculada a la ruta específica del mapa xml, se devuelve una lista vacía si no hay nada mapeado/vinculado.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Representa el filtro automático para la hoja de cálculo especificada.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Obtiene la imagen de fondo de la hoja de cálculo.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Obtiene la colección de celdas en esta hoja de cálculo que se están observando en la 'ventana de observación'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Obtiene la colección de [Cells](../../com.aspose.cells/cells).

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Obtiene una colección de [Chart](../../com.aspose.cells/chart)

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Obtiene una colección de [CheckBox](../../com.aspose.cells/checkbox).

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
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


Obtiene el nombre de código de la hoja de cálculo.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Obtiene la colección de [Comment](../../com.aspose.cells/comment).

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Obtiene los ConditionalFormattings en la hoja de cálculo.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Obtiene un objeto que representa la información de identificador asociada a una hoja de cálculo.

**Remarks**

Worksheet.CustomProperties proporciona un mecanismo preferido para almacenar datos arbitrarios. Soporta componentes de documentos de terceros heredados, así como aquellas situaciones que requieren estrictamente partes binarias.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
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
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Obtiene la configuración de verificación de errores aplicada a ciertos rangos.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
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
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtiene el color de la línea de cuadrícula

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Obtiene la colección de [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection).

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Obtiene la colección de [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection).

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de la hoja en la colección de hojas de cálculo.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Obtiene todos los ListObjects en esta hoja de cálculo.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la hoja de cálculo.

**Remarks**

La longitud máxima del nombre de la hoja es 31. Y no puede asignar el mismo nombre (sin distinción de mayúsculas) a dos hojas de cálculo. Por ejemplo, no puede establecer "SheetName1" en la primera hoja y "SHEETNAME1" en la segunda hoja.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Representa una colección de [OleObject](../../com.aspose.cells/oleobject) en una hoja de cálculo.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Obtiene el contorno en esta hoja de cálculo.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Representa la descripción de la configuración de página en esta hoja.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Indica si el panel tiene divisiones horizontales o verticales, y si esas divisiones están congeladas.

Ver [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Obtiene los paneles de ventana.

**Remarks**

Si la ventana no está dividida o congelada.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Obtiene una colección de [Picture](../../com.aspose.cells/picture).

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Obtiene todas las tablas dinámicas en esta hoja de cálculo.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Obtiene saltos de página automáticos.

**Remarks**

Cada área de celda representa una hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Las opciones de impresión |

**Returns:**
com.aspose.cells.CellArea[] - Las áreas de saltos de página automáticos.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo. Soporta opciones de protección avanzadas en ExcelXP y versiones posteriores.

**Remarks**

Esta propiedad puede proteger la hoja de cálculo en todas las versiones de archivos Excel y soporta opciones de protección avanzadas en ExcelXP y versiones posteriores.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Obtiene [QueryTableCollection](../../com.aspose.cells/querytablecollection) en la hoja de cálculo.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Obtiene la colección de [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador.

**Returns:**
com.aspose.cells.Range[] - Devuelve todos los rangos seleccionados.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Worksheet.GetSelectedAreas(). Esta propiedad será eliminada 12 meses después desde marzo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.util.ArrayList - Una ArrayList que contiene los rangos seleccionados.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Devuelve todas las formas de dibujo en esta hoja de cálculo.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Indica si se deben mostrar los íconos de tipo de datos.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Indica si se deben mostrar las fórmulas o sus resultados.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Obtiene la colección de Slicer en la hoja de cálculo

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Obtiene todos los objetos de [SmartTagCollection](../../com.aspose.cells/smarttagcollection) de la hoja de cálculo.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Obtiene los grupos de sparkline en la hoja de cálculo.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Representa el color de la pestaña de la hoja de cálculo.

**Remarks**

Esta característica solo es compatible con ExcelXP (Excel2002) y versiones posteriores. Si guarda el archivo en formato Excel97 o Excel2000, se omitirá.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Especifica el identificador interno de la hoja.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Obtiene una colección de [TextBox](../../com.aspose.cells/textbox).

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Obtiene la colección de Timeline en la hoja de cálculo

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Indica si la opción de Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Indica si la opción de Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de hoja de cálculo.

Ver [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Obtiene el id único, es el mismo que \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Obtiene la colección de [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection).

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Obtiene el tipo de vista.

Ver [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Indica el estado visible de esta hoja.

Ver [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtiene el objeto del libro de trabajo que contiene esta hoja.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Remarks**

Por favor, establezca primero el tipo de vista.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Indica si esta hoja de cálculo tiene filtro automático.

**Returns:**
boolean
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


Obtiene un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Indica si se muestra el contorno.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica si la hoja de cálculo está protegida.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Obtiene un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. El valor predeterminado es true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Indica si la regla es visible. Esta propiedad solo se aplica a la vista previa de salto de página.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indica si esta hoja de cálculo está seleccionada cuando se abre el libro.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representa si la hoja de cálculo es visible.

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




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Protege la hoja de cálculo.

**Remarks**

Este método protege la hoja de cálculo sin contraseña. Puede proteger la hoja de cálculo en todas las versiones del archivo de Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Protege la hoja de cálculo.

**Remarks**

Este método puede proteger la hoja de cálculo en todas las versiones del archivo de Excel.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección. |
| password | java.lang.String | Contraseña. |
| oldPassword | java.lang.String | Si la hoja de cálculo ya está protegida con una contraseña, proporcione la contraseña anterior. De lo contrario, puede establecer un valor nulo o una cadena vacía para este parámetro. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Actualiza todas las tablas dinámicas en esta hoja de cálculo.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Actualiza todas las tablas dinámicas en esta hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | La opción para actualizar la fuente de datos de la tabla dinámica. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Elimina todos los objetos de dibujo en esta hoja de cálculo.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Elimina el filtro automático de la hoja de cálculo.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Elimina la ventana dividida.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Reemplaza el texto de todas las celdas con una nueva cadena.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldString | java.lang.String | Valor de cadena antiguo. |
| newString | java.lang.String | Valor de cadena nuevo. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Selecciona un rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial |
| totalRows | int | El número de filas. |
| totalColumns | int | El número de columnas |
| removeOthers | boolean | True indica que se eliminan los demás rangos seleccionados y solo se selecciona este rango. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Establece la celda activa en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Establece la imagen de fondo de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Obtiene el nombre de código de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Establece el color de la línea de cuadrícula

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
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

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Indica si la hoja de cálculo especificada se muestra en vista normal o en vista previa de salto de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Establece un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Indica si la regla es visible. Esta propiedad solo se aplica a la vista previa de salto de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica si esta hoja de cálculo está seleccionada cuando se abre el libro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Indica si se deben mostrar los íconos de tipo de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Indica si se deben mostrar las fórmulas o sus resultados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Representa el color de la pestaña de la hoja de cálculo.

**Remarks**

Esta característica solo es compatible con ExcelXP (Excel2002) y versiones posteriores. Si guarda el archivo en formato Excel97 o Excel2000, se omitirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Especifica el identificador interno de la hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Indica si la opción de Entrada de Fórmula de Transición (compatibilidad con Lotus) está habilitada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Indica si la opción de Evaluación de Fórmula de Transición (compatibilidad con Lotus) está habilitada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representa el tipo de hoja de cálculo.

Ver [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Establece el id único, es el mismo que \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Establece el tipo de vista.

Ver [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Indica el estado visible de esta hoja.

Ver [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representa si la hoja de cálculo es visible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Establece las opciones visibles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVisible | boolean | Si la hoja de cálculo es visible |
| ignoreError | boolean | Si se debe ignorar el error cuando esta opción no es válida. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Remarks**

Por favor, establezca primero el tipo de vista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### split() {#split--}
```
public void split()
```


Divide la ventana.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Inicia la sesión que usa cachés para acceder a los datos en esta hoja de cálculo.

**Remarks**

Después de terminar el acceso a los datos, [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) debe invocarse con las mismas opciones para borrar todas las cachés y recuperar el modo de acceso normal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opciones de acceso a datos |

### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Worksheet actual.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Descongela los paneles en la hoja de cálculo.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Desprotege la hoja de cálculo.

**Remarks**

Este método desprotege la hoja de cálculo que está protegida sin contraseña.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Desprotege la hoja de cálculo.

**Remarks**

Si la hoja de cálculo está protegida sin una contraseña, puede establecer un valor nulo o una cadena vacía en el parámetro de contraseña.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | Contraseña |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Consulta áreas de celdas que están mapeadas/vinculadas a la ruta específica del mapa XML.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Worksheet.GetAreasOfXmlMapQuery(). Esta propiedad será eliminada 12 meses después desde agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | ruta del elemento xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Especifique un mapa xml si desea consultar la ruta específica dentro de un mapa específico |

**Returns:**
java.util.ArrayList - lista de [CellArea](../../com.aspose.cells/cellarea) que está mapeada/vinculada a la ruta específica del mapa xml, se devuelve una lista vacía si no hay nada mapeado/vinculado.
