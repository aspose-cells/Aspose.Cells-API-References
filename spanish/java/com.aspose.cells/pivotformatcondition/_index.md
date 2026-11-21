---
title: "PivotFormatCondition"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una condición de formato de PivotTable en la colección PivotFormatCondition."
type: docs
url: /es/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Representa una condición de formato de PivotTable en la colección PivotFormatCondition.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use la clase [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat). Este método será eliminado 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Example**

```
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Agrega el límite de formato condicional de PivotTable en los campos de columna. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Agrega el límite de formato condicional de PivotTable en los campos de columna. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Agrega el límite de formato condicional de PivotTable en los campos de datos. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Agrega el límite de formato condicional de PivotTable en los campos de datos. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Agrega el límite de formato condicional de PivotTable en los campos de fila. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Agrega el límite de formato condicional de PivotTable en los campos de fila. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Obtiene las condiciones del formato condicional de la tabla dinámica. |
| [getRuleType()](#getRuleType--) | Obtiene el tipo de regla para el formato condicional de la tabla dinámica. |
| [getScopeType()](#getScopeType--) | Obtiene el tipo de alcance para el formato condicional de la tabla dinámica. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Establece las áreas condicionales del objeto PivotFormatCondition. |
| [setRuleType(int value)](#setRuleType-int-) | Establece el tipo de regla para el formato condicional de la tabla dinámica. |
| [setScopeType(int value)](#setScopeType-int-) | Establece el tipo de alcance para el formato condicional de la tabla dinámica. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Agrega el límite de formato condicional de PivotTable en los campos de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | El PivotField en los campos de columna. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Agrega el límite de formato condicional de PivotTable en los campos de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | java.lang.String | El nombre de PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Agrega el límite de formato condicional de PivotTable en los campos de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | El PivotField en los campos de datos. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Agrega el límite de formato condicional de PivotTable en los campos de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | java.lang.String | El nombre de PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Agrega el límite de formato condicional de PivotTable en los campos de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | El PivotField en los campos de fila. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Agrega el límite de formato condicional de PivotTable en los campos de fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | java.lang.String | El nombre de PivotField. |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Obtiene las condiciones del formato condicional de la tabla dinámica.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Obtiene el tipo de regla para el formato condicional de la tabla dinámica.

Ver [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Obtiene el tipo de alcance para el formato condicional de la tabla dinámica.

Ver [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Returns:**
int
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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Establece las áreas condicionales del objeto PivotFormatCondition.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Establece el tipo de regla para el formato condicional de la tabla dinámica.

Ver [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Establece el tipo de alcance para el formato condicional de la tabla dinámica.

Ver [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

