---
title: "RevisionCustomView"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un record di revisione dell'aggiunta o rimozione di una vista personalizzata alla cartella di lavoro"
type: docs
url: /it/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

Rappresenta un record di revisione dell'aggiunta o rimozione di una vista personalizzata alla cartella di lavoro
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Restituisce il tipo di azione. |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | Restituisce l'identificatore univoco globale della vista personalizzata. |
| [getId()](#getId--) | Ottiene il numero di questa revisione. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Restituisce il tipo di azione.

Vedi [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Restituisce l'identificatore univoco globale della vista personalizzata.

**Returns:**
java.util.UUID
### getId() {#getId--}
```
public int getId()
```


Ottiene il numero di questa revisione.

**Remarks**

Zero indica che questa revisione non contiene ID.

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

