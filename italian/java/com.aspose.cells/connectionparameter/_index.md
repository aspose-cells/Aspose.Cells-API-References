---
title: "ConnectionParameter"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica le proprietà di eventuali parametri utilizzati con connessioni dati esterne. I parametri sono validi per query ODBC e web."
type: docs
url: /it/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Specifica le proprietà di eventuali parametri utilizzati con connessioni dati esterne. I parametri sono validi per query ODBC e web.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Il nome del parametro. |
| [getPrompt()](#getPrompt--) | Stringa di prompt per il parametro. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. |
| [getSqlType()](#getSqlType--) | Tipo di dati SQL del parametro. |
| [getType()](#getType--) | Tipo di parametro utilizzato. |
| [getValue()](#getValue--) | Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. |
| [setName(String value)](#setName-java.lang.String-) | Il nome del parametro. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Stringa di prompt per il parametro. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. |
| [setSqlType(int value)](#setSqlType-int-) | Tipo di dati SQL del parametro. |
| [setType(int value)](#setType-int-) | Tipo di parametro utilizzato. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Il nome del parametro.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se vero, i dati esterni vengono aggiornati utilizzando il nuovo valore del parametro ogni volta che si verifica una modifica. Se falso, i dati esterni vengono aggiornati solo su richiesta dell'utente o quando qualche altro evento attiva l'aggiornamento (ad es., apertura della cartella di lavoro).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


Tipo di dati SQL del parametro. Valido solo per le origini ODBC.

Vedi [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Tipo di parametro utilizzato. Se parameterType=valore, verrà utilizzato il valore da boolean, double, integer o string. In questo caso, ci si aspetta che venga specificato solo uno tra \{boolean, double, integer, or string\}.

Vedi [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Valore numerico non intero, valore intero, valore stringa o valore Boolean da utilizzare come parametro della query. Utilizzato solo quando parameterType è value.

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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Il nome del parametro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se vero, i dati esterni vengono aggiornati utilizzando il nuovo valore del parametro ogni volta che si verifica una modifica. Se falso, i dati esterni vengono aggiornati solo su richiesta dell'utente o quando qualche altro evento attiva l'aggiornamento (ad es., apertura della cartella di lavoro).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


Tipo di dati SQL del parametro. Valido solo per le origini ODBC.

Vedi [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Tipo di parametro utilizzato. Se parameterType=valore, verrà utilizzato il valore da boolean, double, integer o string. In questo caso, ci si aspetta che venga specificato solo uno tra \{boolean, double, integer, or string\}.

Vedi [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Valore numerico non intero, valore intero, valore stringa o valore Boolean da utilizzare come parametro della query. Utilizzato solo quando parameterType è value.

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

