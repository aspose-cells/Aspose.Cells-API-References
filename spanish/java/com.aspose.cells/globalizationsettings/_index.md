---
title: "GlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración de globalización."
type: docs
url: /es/java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Representa la configuración de globalización.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compara dos valores de cadena según ciertas reglas de ordenación. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Obtiene el nombre de la etiqueta "(All)" en la tabla dinámica. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Obtiene el valor de cadena de visualización para el valor booleano de la celda |
| [getChartSettings()](#getChartSettings--) | Obtiene la configuración de globalización para el gráfico. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforma la cadena en un objeto comparable según ciertas reglas de ordenación. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Obtiene el nombre de la etiqueta "Column Labels" en la tabla dinámica. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título del comentario. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Obtiene el nombre del encabezado del campo del área de valores en la tabla dinámica. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. |
| [getEmptyDataName()](#getEmptyDataName--) | Obtiene el nombre de la etiqueta "(blank)" en la tabla dinámica. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Obtiene el valor de cadena de visualización para el valor de error de la celda |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Obtiene el nombre del total general de la función. |
| [getListSeparator()](#getListSeparator--) | Obtiene el separador para listas, parámetros de la función, ...etc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Obtiene el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Obtiene el nombre de la etiqueta "(Multiple Items)" en la tabla dinámica. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Obtiene el nombre de la etiqueta "Grand Total" en la tabla dinámica. |
| [getPivotSettings()](#getPivotSettings--) | Obtiene la configuración de globalización para la tabla dinámica. |
| [getPivotTotalName()](#getPivotTotalName--) | Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Obtiene el nombre de protección en la tabla dinámica. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Obtiene el separador para filas en datos de matriz en la fórmula. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Obtiene el nombre estándar en inglés del estilo de fuente (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Obtiene el nombre del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) en la tabla dinámica. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Obtiene el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Obtiene el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Obtiene el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada. |
| [getTotalName(int functionType)](#getTotalName-int-) | Obtiene el nombre total de la función. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Establece la configuración de globalización para el gráfico. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Establece la configuración de globalización para la tabla dinámica. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Compara dos valores de cadena según ciertas reglas de ordenación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v1 | java.lang.String | la primera cadena |
| v2 | java.lang.String | la segunda cadena |
| ignoreCase | boolean | si se ignora mayúsculas y minúsculas al comparar valores |

**Returns:**
int - Entero que indica la relación léxica entre los dos comparandos
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Obtiene el nombre de la etiqueta "(All)" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método GlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String - El nombre de la etiqueta "(All)" label
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Obtiene el valor de cadena de visualización para el valor booleano de la celda

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bv | boolean | valor booleano |

**Returns:**
java.lang.String - Por defecto devuelve "TRUE" para el valor verdadero y "FALSE" para el valor falso.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Obtiene la configuración de globalización para el gráfico.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transforma la cadena en un objeto comparable según ciertas reglas de ordenación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v | java.lang.String | El valor de cadena necesita compararse con otros. |
| ignoreCase | boolean | si se ignora mayúsculas y minúsculas al comparar valores |

**Returns:**
java.lang.Comparable - El objeto puede usarse para comparar o ordenar valores de cadena
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Obtiene el nombre de la etiqueta "Column Labels" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de las etiquetas de columna
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título del comentario.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). |

**Returns:**
java.lang.String -
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Obtiene el nombre del encabezado del campo del área de valores en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre del encabezado del campo de datos
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El predeterminado es "Sheet".

**Remarks**

El nombre de la hoja agregada automáticamente (por ejemplo mediante [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\\#add--)) será el nombre especificado más un número de secuencia. Por ejemplo, un usuario de Alemania podría querer que el nombre de la hoja sea "Tabellenblatt2" en lugar de "Sheet2". Entonces el usuario puede implementar este método para devolver "Tabellenblatt".

**Returns:**
java.lang.String - el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Obtiene el nombre de la etiqueta "(blank)" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de datos vacíos
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Obtiene el valor de cadena de visualización para el valor de error de la celda

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| err | java.lang.String | valores de error como \\#VALUE!,\\#NAME? |

**Returns:**
java.lang.String - Por defecto devuelve el propio valor de error
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Obtiene el nombre del total general de la función.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). El tipo de función. |

**Returns:**
java.lang.String - El nombre del total general de la función.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Obtiene el separador para listas, parámetros de la función, ...etc.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) texto del nombre incorporado. |

**Returns:**
java.lang.String - Texto dependiente de la configuración regional. La configuración regional fue especificada por el Libro de trabajo para el cual se usa esta configuración.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Obtiene el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) nombre de la función. |

**Returns:**
java.lang.String - Nombre de función dependiente de la configuración regional. La configuración regional fue especificada por el Libro de trabajo para el cual se usa esta configuración.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Obtiene el nombre de la etiqueta "(Multiple Items)" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de la etiqueta "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Obtiene el nombre de la etiqueta "Grand Total" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de la etiqueta "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Obtiene la configuración de globalización para la tabla dinámica.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de la etiqueta "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Obtiene el nombre de protección en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetTextOfProtectedName(string). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String - El nombre de protección de la tabla dinámica
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String - El nombre de las etiquetas de fila
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Obtiene el separador para filas en datos de matriz en la fórmula.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | java.lang.String | Texto dependiente de la configuración regional del nombre incorporado. La configuración regional fue especificada por el Workbook para el cual se usa esta configuración. |

**Returns:**
java.lang.String - Texto estándar (configuración regional en-US).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | java.lang.String | Nombre de función dependiente de la configuración regional. La configuración regional fue especificada por el Workbook para el cual se usa esta configuración. |

**Returns:**
java.lang.String - Nombre de función estándar (configuración regional en-US).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Obtiene el nombre estándar en inglés del estilo de fuente (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Nombre de estilo de fuente dependiente de la configuración regional para Header/Footer. |

**Returns:**
java.lang.String - Nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Obtiene el nombre del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). El tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - El nombre del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Obtiene el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. El valor predeterminado es "All", por lo que en la fórmula "\#All" representa todas las filas de la tabla referenciada.

**Returns:**
java.lang.String - el nombre del tipo de filas de tabla
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. El valor predeterminado es "This Row", por lo que en la fórmula "\#This Row" representa la fila actual de la tabla referenciada.

**Returns:**
java.lang.String - el nombre del tipo de filas de tabla
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El valor predeterminado es "Data", por lo que en la fórmula "\#Data" representa la región de datos de la tabla.

**Returns:**
java.lang.String - el nombre del tipo de filas de tabla
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Obtiene el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. El valor predeterminado es "Headers", por lo que en la fórmula "\#Headers" representa el encabezado de la tabla.

**Returns:**
java.lang.String - el nombre del tipo de filas de tabla
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Obtiene el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada. El valor predeterminado es "Totals", por lo que en la fórmula "\#Totals" representa la fila total de la tabla referenciada.

**Returns:**
java.lang.String - el nombre del tipo de filas de tabla
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Obtiene el nombre total de la función.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). El tipo de función. |

**Returns:**
java.lang.String - El nombre total de la función.
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




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Establece la configuración de globalización para el gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Establece la configuración de globalización para la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

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

