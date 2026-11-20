---
title: "RowColumnEventArgs"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce dati per gli eventi riga/colonna."
type: docs
url: /it/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Fornisce dati per gli eventi riga/colonna.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | L'argomento dell'evento. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Il numero di riga o colonna, inizia da zero. |
| [getType()](#getType--) | Il tipo di riga o colonna. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | Dobbiamo annullare l'operazione. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Chiama questo metodo nei gestori di eventi RowDeleting/ColumnDeleting per annullare le operazioni di eliminazione. |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


L'argomento dell'evento.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


Il numero di riga o colonna, inizia da zero.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Il tipo di riga o colonna.

Vedi [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


Dobbiamo annullare l'operazione.

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




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


Chiama questo metodo nei gestori di eventi RowDeleting/ColumnDeleting per annullare le operazioni di eliminazione.

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

