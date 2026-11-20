---
title: "RevisionInsertDelete"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un record di revisione di un'azione di inserimento/eliminazione di riga/colonna."
type: docs
url: /it/java/com.aspose.cells/revisioninsertdelete/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```

Rappresenta un record di revisione di un'azione di inserimento/eliminazione di riga/colonna.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Ottiene il tipo di azione di questa revisione. |
| [getCellArea()](#getCellArea--) | Ottiene l'intervallo di inserimento/cancellazione. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Ottiene il numero di questa revisione. |
| [getRevisions()](#getRevisions--) | Ottiene l'elenco delle revisioni per questa operazione. |
| [getType()](#getType--) | Rappresenta il tipo di revisione. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Ottiene il tipo di azione di questa revisione.

Vedi [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ottiene l'intervallo di inserimento/cancellazione.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```


Ottiene l'elenco delle revisioni per questa operazione.

**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di revisione.

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

