---
title: "CellValue"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il valore della cella e il tipo corrispondente."
type: docs
url: /it/java/com.aspose.cells/cellvalue/
---

**Inheritance:**
java.lang.Object
```
public class CellValue
```

Rappresenta il valore della cella e il tipo corrispondente.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Restituisce il tipo del valore di cella. |
| [getValue()](#getValue--) | Restituisce il valore della cella. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | Imposta il tipo del valore di cella. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore della cella. |
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
| Parametro | Tipo | Descrizione |
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


Restituisce il tipo del valore di cella.

Vedi [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore della cella.

**Remarks**

Il valore deve essere del tipo corretto di oggetto corrispondente a [getType()](../../com.aspose.cells/cellvalue\#getType--):

| Tipo | Valore |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, qualsiasi altro oggetto verrà ignorato |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | string di errore come "\#VALUE!", "\#NAME?", ... |

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


Imposta il tipo del valore di cella.

Vedi [CellValueType](../../com.aspose.cells/cellvaluetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Imposta il valore della cella.

**Remarks**

Il valore deve essere del tipo corretto di oggetto corrispondente a [getType()](../../com.aspose.cells/cellvalue\#getType--):

| Tipo | Valore |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, qualsiasi altro oggetto verrà ignorato |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | string di errore come "\#VALUE!", "\#NAME?", ... |

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

