---
title: "PivotAreaFilter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el filtro de  para ."
type: docs
url: /es/java/com.aspose.cells/pivotareafilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotAreaFilter
```

Representa el filtro de [PivotArea](../../com.aspose.cells/pivotarea) para [PivotTable](../../com.aspose.cells/pivottable).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PivotAreaFilter()](#PivotAreaFilter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Obtiene el índice del campo en los campos de origen al que se refiere este filtro. |
| [getSelected()](#getSelected--) | Indica si este campo tiene selección. |
| [hashCode()](#hashCode--) |  |
| [isSubtotalSet(int subtotalType)](#isSubtotalSet-int-) | Obtiene qué subtotal está establecido para este filtro. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica si este campo tiene selección. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Subtotal para el filtro. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotAreaFilter() {#PivotAreaFilter--}
```
public PivotAreaFilter()
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
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Obtiene el índice del campo en los campos de origen al que se refiere este filtro. Un valor de -2 indica el campo de valores.

**Returns:**
int
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Indica si este campo tiene selección. Solo funciona cuando la tabla dinámica está en vista de esquema.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSubtotalSet(int subtotalType) {#isSubtotalSet-int-}
```
public boolean isSubtotalSet(int subtotalType)
```


Obtiene qué subtotal está establecido para este filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). El tipo de función de subtotal. |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica si este campo tiene selección. Solo funciona cuando la tabla dinámica está en vista de esquema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Subtotal para el filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). La función de subtotal. |
| mostrado | boolean | Indica si se muestra este dato de subtotal. |

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

