---
title: "RevisionCellChange"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la revisione che modifica le celle."
type: docs
url: /it/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Rappresenta la revisione che modifica le celle.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Restituisce il nome della cella. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Restituisce l'indice della colonna della cella. |
| [getId()](#getId--) | Ottiene il numero di questa revisione. |
| [getNewFormula()](#getNewFormula--) | Restituisce la formula precedente. |
| [getNewStyle()](#getNewStyle--) | Ottiene il nuovo stile della cella. |
| [getNewValue()](#getNewValue--) | Ottiene il nuovo valore della cella. |
| [getOldFormula()](#getOldFormula--) | Restituisce la formula precedente. |
| [getOldStyle()](#getOldStyle--) | Ottiene lo stile precedente della cella. |
| [getOldValue()](#getOldValue--) | Ottiene il valore precedente della cella. |
| [getRow()](#getRow--) | Restituisce l'indice della riga della cella. |
| [getType()](#getType--) | Rappresenta il tipo di revisione. |
| [getWorksheet()](#getWorksheet--) | Ottiene il foglio di lavoro. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Indica se questa cella è formattata come nuova. |
| [isOldFormatted()](#isOldFormatted--) | Indica se questa cella è formattata come vecchia. |
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


Restituisce l'indice della colonna della cella.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Restituisce la formula precedente.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Ottiene il nuovo stile della cella.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Ottiene il nuovo valore della cella.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Restituisce la formula precedente.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Ottiene lo stile precedente della cella.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Ottiene il valore precedente della cella.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce l'indice della riga della cella.

**Returns:**
int
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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Indica se questa cella è formattata come nuova.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Indica se questa cella è formattata come vecchia.

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

