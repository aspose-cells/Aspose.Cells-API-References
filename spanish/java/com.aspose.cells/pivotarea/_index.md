---
title: "PivotArea"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Presenta el área seleccionada de la tabla dinámica."
type: docs
url: /es/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Presenta el área seleccionada de la tabla dinámica.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Presenta el área seleccionada de la tabla dinámica. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Obtiene la región de la tabla dinámica a la que se aplica esta regla. |
| [getCellAreas()](#getCellAreas--) | Obtiene las áreas de celdas de esta área dinámica. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Obtiene todos los filtros para este PivotArea. |
| [getOnlyData()](#getOnlyData--) | Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento. |
| [getOnlyLabel()](#getOnlyLabel--) | Indica si solo se seleccionan las etiquetas de datos para una selección de elemento. |
| [getRuleType()](#getRuleType--) | Obtiene el tipo de regla de selección. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Indica si se incluye el total general de la columna. |
| [isOutline()](#isOutline--) | Indica si la regla se refiere a un área que está en modo de esquema. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Indica si se incluye el total general de la fila. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Seleccione el área con filtros. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Seleccione un campo en la región como área. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Seleccione un campo en la región como área. |
| [setAxisType(int value)](#setAxisType-int-) | Establece la región de la tabla dinámica a la que se aplica esta regla. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Indica si se incluye el total general de la columna. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Indica si solo se seleccionan las etiquetas de datos para una selección de elemento. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indica si la regla se refiere a un área que está en modo de esquema. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Indica si se incluye el total general de la fila. |
| [setRuleType(int value)](#setRuleType-int-) | Establece el tipo de regla de selección. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Presenta el área seleccionada de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Obtiene la región de la tabla dinámica a la que se aplica esta regla.

Ver [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Obtiene las áreas de celdas de esta área dinámica.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


Obtiene todos los filtros para este PivotArea.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Indica si solo se seleccionan las etiquetas de datos para una selección de elemento.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Obtiene el tipo de regla de selección.

Ver [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


Indica si se incluye el total general de la columna.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Indica si la regla se refiere a un área que está en modo de esquema.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Indica si se incluye el total general de la fila.

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


Seleccione el área con filtros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La región de la tabla dinámica a la que se aplica esta regla. |
| fieldPosition | int | Posición del campo dentro del eje al que se aplica esta regla. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Especifica qué se puede seleccionar en una tabla dinámica durante una selección estructurada. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Seleccione un campo en la región como área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de región. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | El campo de tabla dinámica. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Seleccione un campo en la región como área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). El tipo de región. |
| fieldName | java.lang.String | El nombre del campo de tabla dinámica. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Establece la región de la tabla dinámica a la que se aplica esta regla.

Ver [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Indica si se incluye el total general de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Indica si solo se seleccionan las etiquetas de datos para una selección de elemento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indica si la regla se refiere a un área que está en modo de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Indica si se incluye el total general de la fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Establece el tipo de regla de selección.

Ver [PivotAreaType](../../com.aspose.cells/pivotareatype).

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

