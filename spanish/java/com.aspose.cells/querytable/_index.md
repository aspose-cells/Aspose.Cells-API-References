---
title: "QueryTable"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la información de QueryTable."
type: docs
url: /es/java/com.aspose.cells/querytable/
---

**Inheritance:**
java.lang.Object
```
public class QueryTable
```

Representa la información de QueryTable.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Getting the first query table in the worksheet if exists
         //QueryTable qt = worksheet.QueryTables[0];
         //Getting display address of the query table.
         //string address = qt.ResultRange.Address;
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | Devuelve o establece el AdjustColumnWidth del objeto. |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | Obtiene el id de conexión de la tabla de consulta. |
| [getExternalConnection()](#getExternalConnection--) | Obtiene la conexión externa relacionada. |
| [getName()](#getName--) | Obtiene el nombre de la tabla de consulta. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Devuelve o establece el PreserveFormatting del objeto. |
| [getResultRange()](#getResultRange--) | Obtiene el rango del resultado. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | Devuelve o establece el AdjustColumnWidth del objeto. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Devuelve o establece el PreserveFormatting del objeto. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```


Devuelve o establece el AdjustColumnWidth del objeto.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Obtiene el id de conexión de la tabla de consulta.

**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```


Obtiene la conexión externa relacionada.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la tabla de consulta.

**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Devuelve o establece el PreserveFormatting del objeto.

**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```


Obtiene el rango del resultado.

**Returns:**
[Range](../../com.aspose.cells/range) - 
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




### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```


Devuelve o establece el AdjustColumnWidth del objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Devuelve o establece el PreserveFormatting del objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

