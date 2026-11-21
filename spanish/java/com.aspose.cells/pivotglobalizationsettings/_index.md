---
title: "PivotGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la configuración de globalización para tablas dinámicas."
type: docs
url: /es/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

Representa la configuración de globalización para tablas dinámicas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Obtiene el formato numérico del grupo de día de la tabla dinámica. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Obtiene el nombre para mostrar del campo de datos de la tabla dinámica. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Obtiene todas las cadenas de formato corto de los 12 meses. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Obtiene todas las cadenas con formato local de las 24 horas. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Obtiene el texto local de los 4 trimestres. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Obtiene el texto local de los 4 trimestres. |
| [getTextOfAll()](#getTextOfAll--) | Obtiene el texto de la etiqueta "(All)" en la tabla dinámica. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Obtiene el texto localizado de "All Periods". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Obtiene el texto de la etiqueta "Column Labels" en la tabla dinámica. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Obtiene el texto del encabezado del campo del área de valores en la tabla dinámica. |
| [getTextOfDays()](#getTextOfDays--) | Obtiene el texto local de "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Obtiene el texto de la etiqueta "(blank)" en la tabla dinámica. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Obtiene el texto de la etiqueta "Grand Total" en la tabla dinámica. |
| [getTextOfHours()](#getTextOfHours--) | Obtiene el texto local de "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | Obtiene el texto local de "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | Obtiene el texto local de "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Obtiene el texto de la etiqueta "(Multiple Items)" en la tabla dinámica. |
| [getTextOfOr()](#getTextOfOr--) | Obtiene todas las cadenas formateadas localmente de "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Obtiene el texto para el nombre protegido especificado. |
| [getTextOfProtection()](#getTextOfProtection--) | Obtiene el nombre de protección en la tabla dinámica. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Obtiene el texto local de "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | Obtiene el texto local de "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Obtiene el texto de la etiqueta "Row Labels" en la tabla dinámica. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Obtiene el texto local de "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Obtiene el texto del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) en la tabla dinámica. |
| [getTextOfTotal()](#getTextOfTotal--) | Obtiene el texto de la etiqueta "Total" en la tabla dinámica. |
| [getTextOfYears()](#getTextOfYears--) | Obtiene el texto local de "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Obtiene el formato numérico del grupo de día de tabla dinámica. Solo se usa al agrupar el campo de tabla dinámica por días. El valor predeterminado es "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Obtiene el nombre para mostrar del campo de datos de tabla dinámica. El formato predeterminado es "Sum Of Field".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La función se usa para resumir los valores del campo de tabla dinámica. |
| name | java.lang.String | El nombre original del campo de tabla dinámica. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Obtiene todas las cadenas de formato corto de los 12 meses.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Obtiene todas las cadenas formateadas localmente de 24 horas. El valor predeterminado es 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Obtiene el texto local de los 4 trimestres.

**Remarks**

Por defecto devuelve Quarter1, Quarter2, Quarter3, Quarter4 antes de la versión 26.9. Por defecto devuelve Qtr1, Qtr2, Qtr3, Qtr4 desde la versión 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Obtiene el texto local de los 4 trimestres.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetTextOf4Quarters(). Esta propiedad será eliminada 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Obtiene el texto de la etiqueta "(All)" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de la etiqueta "(All)"
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Obtiene el texto localizado de "All Periods".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Obtiene el texto de la etiqueta "Column Labels" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de las etiquetas de columna
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Obtiene el texto del encabezado del campo del área de valores en la tabla dinámica.

**Returns:**
java.lang.String - El texto del nombre del encabezado del campo de datos
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Obtiene el texto local de "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Obtiene el texto de la etiqueta "(blank)" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de datos vacíos
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Obtiene el texto de la etiqueta "Grand Total" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de la etiqueta "Grand Total"
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Obtiene el texto local de "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Obtiene el texto local de "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Obtiene el texto local de "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Obtiene el texto de la etiqueta "(Multiple Items)" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de la etiqueta "(Multiple Items)"
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Obtiene todas las cadenas formateadas localmente de "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Obtiene el texto para el nombre protegido especificado.

**Remarks**

En Ms Excel, algunos nombres no pueden usarse como nombre de PivotFields en una PivotTable. Varían según la región; el usuario puede especificarlos explícitamente de acuerdo con la región utilizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectedName | java.lang.String | El nombre protegido en la PivotTable. |

**Returns:**
java.lang.String - Los nombres locales protegidos de la PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Obtiene el nombre de protección en la tabla dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetTextOfProtectedName(string). Esta propiedad será eliminada 12 meses después a partir de marzo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String - El nombre de protección de la tabla dinámica
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Obtiene el texto local de "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Obtiene el texto local de "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Obtiene el texto de la etiqueta "Row Labels" en la tabla dinámica.

**Returns:**
java.lang.String - El texto de las etiquetas de fila
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Obtiene el texto local de "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Obtiene el texto del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) en la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). El [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - El texto del tipo dado
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Obtiene el texto de la etiqueta "Total" en la PivotTable. Necesita sobrescribir este método cuando la PivotTable contiene dos o más PivotFields en el área de datos.

**Returns:**
java.lang.String - El texto de la etiqueta "Total"
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Obtiene el texto local de "Years".

**Returns:**
java.lang.String -
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

