---
title: "ReferredArea"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un'area di riferimento nella formula."
type: docs
url: /it/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

Rappresenta un'area di riferimento nella formula.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | La colonna finale dell'area. |
| [getEndRow()](#getEndRow--) | La riga finale dell'area. |
| [getExternalFileName()](#getExternalFileName--) | Ottieni il nome del file esterno se questa è un riferimento esterno. |
| [getSheetName()](#getSheetName--) | Indica in quale foglio si trova questo riferimento. |
| [getSheetNames()](#getSheetNames--) | Nomi di tutti i fogli di lavoro a cui questa istanza fa riferimento. |
| [getStartColumn()](#getStartColumn--) | La colonna iniziale dell'area. |
| [getStartRow()](#getStartRow--) | La riga iniziale dell'area. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Ottiene il valore della cella con l'offset dato dall'angolo superiore sinistro di quest'area. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Ottiene il valore della cella con l'offset dato dall'angolo superiore sinistro di quest'area. |
| [getValues()](#getValues--) | Ottiene i valori delle celle in quest'area. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Ottiene i valori delle celle in quest'area. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indica se questa è un'area. |
| [isEntireColumn()](#isEntireColumn--) | Indica se quest'area contiene tutte le righe(intera colonna). |
| [isEntireRow()](#isEntireRow--) | Indica se quest'area contiene tutte le colonne(intera riga). |
| [isExternalLink()](#isExternalLink--) | Indica se questo è un collegamento esterno. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Restituisce l'indirizzo di riferimento di quest'area. |
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


Ottieni il nome del file esterno se questa è un riferimento esterno.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Indica in quale foglio si trova questo riferimento.

**Remarks**

Se fa riferimento a più fogli di lavoro, il valore restituito è simile all'espressione di intervallo nella formula. Per esempio "Sheet1:Sheet3" per il riferimento nella formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


Nomi di tutti i fogli di lavoro a cui questa istanza fa riferimento.

**Returns:**
java.lang.String[]
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
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


Ottiene il valore della cella con l'offset dato dall'angolo superiore sinistro di quest'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | offset di riga dalla riga iniziale di quest'area |
| colOffset | int | offset di colonna dalla riga iniziale di quest'area |
| calculateFormulas | boolean | Indica se calcolarlo ricorsivamente se il riferimento specificato è una formula. |

**Returns:**
java.lang.Object - "\#REF!" se quest'area è non valida; "\#N/A" se l'offset fornito è fuori da quest'area; altrimenti restituisce il valore della cella nella posizione data.
### getValues() {#getValues--}
```
public Object getValues()
```


Ottiene i valori delle celle in quest'area.

**Returns:**
java.lang.Object - Se quest'area è non valida, verrà restituito "\#REF!"; se quest'area è una singola cella, restituisce l'oggetto valore della cella; altrimenti restituisce un array 2D per tutti i valori in quest'area.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


Ottiene i valori delle celle in quest'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calculateFormulas | boolean | In questo intervallo, se ci sono alcune formule non calcolate, questo flag indica se tali formule devono essere calcolate ricorsivamente. |

**Returns:**
java.lang.Object - Se quest'area è non valida, verrà restituito "\#REF!"; se quest'area è una singola cella, restituisce l'oggetto valore della cella; altrimenti restituisce un array 2D per tutti i valori in quest'area.
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
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


Indica se quest'area contiene tutte le righe(intera colonna).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


Indica se quest'area contiene tutte le colonne(intera riga).

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


Restituisce l'indirizzo di riferimento di quest'area. Generalmente è l'indirizzo del riferimento che può essere usato nella formula, ad esempio "Sheet1!A1:C3".

**Returns:**
java.lang.String - l'indirizzo di riferimento di quest'area.
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

