---
title: "RevisionFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un record di revisione delle informazioni su una modifica di formattazione."
type: docs
url: /it/java/com.aspose.cells/revisionformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionFormat extends Revision
```

Rappresenta un record di revisione delle informazioni su una modifica di formattazione.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | L'intervallo a cui è stata applicata questa formattazione. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Ottiene il numero di questa revisione. |
| [getStyle()](#getStyle--) | Ottiene lo stile applicato. |
| [getType()](#getType--) | Ottiene il tipo di revisione. |
| [getWorksheet()](#getWorksheet--) | Ottiene il foglio di lavoro. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


L'intervallo a cui è stata applicata questa formattazione.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


Ottiene il numero di questa revisione.

**Remarks**

Zero indica che questa revisione non contiene ID.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ottiene lo stile applicato.

**Returns:**
[Style](../../com.aspose.cells/style)
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di revisione.

Vedi [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ottiene il foglio di lavoro.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

