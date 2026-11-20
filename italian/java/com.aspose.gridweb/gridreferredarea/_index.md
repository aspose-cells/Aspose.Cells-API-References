---
title: "GridReferredArea"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un oggetto riferito dalla formula."
type: docs
url: /it/java/com.aspose.gridweb/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```

Rappresenta un oggetto riferito dalla formula.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | La colonna finale dell'area. |
| [getEndRow()](#getEndRow--) | La riga finale dell'area. |
| [getExternalFileName()](#getExternalFileName--) | this.KeepedRels = source.KeepedRels; |
| [getSheetName()](#getSheetName--) | Indica in quale foglio si trova |
| [getStartColumn()](#getStartColumn--) | La colonna iniziale dell'area. |
| [getStartRow()](#getStartRow--) | La riga iniziale dell'area. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Ottiene il valore della cella con l'offset dato dall'angolo superiore sinistro di quest'area. |
| [getValues()](#getValues--) | Ottiene i valori delle celle in quest'area. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indica se questa è un'area. |
| [isExternalLink()](#isExternalLink--) | Indica se questo è un collegamento esterno. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


La colonna finale dell'area.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


La riga finale dell'area.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


this.KeepedRels = source.KeepedRels;

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Indica in quale foglio si trova

**Returns:**
java.lang.String
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


La colonna iniziale dell'area.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


La riga iniziale dell'area.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Ottiene il valore della cella con l'offset dato dall'angolo superiore sinistro di quest'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | offset di riga dalla riga iniziale di quest'area |
| colOffset | int | offset di colonna dalla riga iniziale di quest'area |

**Returns:**
java.lang.Object - "\#REF!" se quest'area è non valida; "\#N/A" se l'offset fornito è fuori da quest'area; altrimenti restituisce il valore della cella nella posizione data.
### getValues() {#getValues--}
```
public Object getValues()
```


Ottiene i valori delle celle in quest'area.

**Returns:**
java.lang.Object - Se quest'area è non valida, verrà restituito "\\#REF!"; Se quest'area è una singola cella, verrà restituito l'oggetto valore della cella; Altrimenti verrà restituito un array per tutti i valori in quest'area.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Indica se questa è un'area.

**Remarks**

Se non si tratta di un'area, hanno effetto solo StartRow e StartColumn.

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Indica se questo è un collegamento esterno.

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

