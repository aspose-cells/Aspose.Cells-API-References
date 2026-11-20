---
title: "RevisionCellComment"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un record di revisione di una modifica al commento di una cella."
type: docs
url: /it/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Rappresenta un record di revisione di una modifica al commento di una cella.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Ottiene il tipo di azione della revisione. |
| [getCellName()](#getCellName--) | Restituisce il nome della cella. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Restituisce l'indice della colonna che contiene un commento. |
| [getId()](#getId--) | Ottiene il numero di questa revisione. |
| [getNewLength()](#getNewLength--) | Restituisce la lunghezza del commento prima che questa revisione fosse effettuata. |
| [getOldLength()](#getOldLength--) | Restituisce la lunghezza del testo del commento aggiunto in questa revisione. |
| [getRow()](#getRow--) | Restituisce l'indice della riga che contiene un commento. |
| [getType()](#getType--) | Ottiene il tipo di revisione. |
| [getWorksheet()](#getWorksheet--) | Ottiene il foglio di lavoro. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Indica se è un commento vecchio. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Restituisce il nome della cella. |
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


Ottiene il tipo di azione della revisione.

Vedi [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


Restituisce il nome della cella.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Restituisce l'indice della colonna che contiene un commento.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Ottiene il numero di questa revisione.

**Remarks**

Zero indica che questa revisione non contiene ID.

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Restituisce la lunghezza del commento prima che questa revisione fosse effettuata.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Restituisce la lunghezza del testo del commento aggiunto in questa revisione.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce l'indice della riga che contiene un commento.

**Returns:**
int
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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Indica se è un commento vecchio.

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Restituisce il nome della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

