---
title: "CellValue"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el valor de la celda y su tipo correspondiente."
type: docs
url: /es/java/com.aspose.cells/cellvalue/
---

**Inheritance:**
java.lang.Object
```
public class CellValue
```

Representa el valor de la celda y su tipo correspondiente.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Obtiene el tipo del valor de celda. |
| [getValue()](#getValue--) | Obtiene el valor de la celda. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | Establece el tipo del valor de celda. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor de la celda. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellValue() {#CellValue--}
```
public CellValue()
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
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo del valor de celda.

Ver [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor de la celda.

**Remarks**

El valor debe ser del tipo correcto de objeto correspondiente al [getType()](../../com.aspose.cells/cellvalue\#getType--):

| Tipo | Value |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, cualquier otro objeto será ignorado |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | cadena de error como "\#VALUE!", "\#NAME?", ... |

**Returns:**
java.lang.Object
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




### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo del valor de celda.

Ver [CellValueType](../../com.aspose.cells/cellvaluetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece el valor de la celda.

**Remarks**

El valor debe ser del tipo correcto de objeto correspondiente al [getType()](../../com.aspose.cells/cellvalue\#getType--):

| Tipo | Value |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, cualquier otro objeto será ignorado |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | cadena de error como "\#VALUE!", "\#NAME?", ... |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

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

