---
title: "CellArea"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un'area di celle."
type: docs
url: /it/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Rappresenta un'area di celle.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Campi

| Campo | Descrizione |
| --- | --- |
| [EndColumn](#EndColumn) | Ottiene o imposta la colonna finale di quest'area. |
| [EndRow](#EndRow) | Ottiene o imposta la riga finale di quest'area. |
| [StartColumn](#StartColumn) | Ottiene o imposta la colonna iniziale di quest'area. |
| [StartRow](#StartRow) | Ottiene o imposta la riga iniziale di quest'area. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Confronta due oggetti CellArea in base al loro angolo in alto a sinistra. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Crea un'area di celle. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Crea un'area di celle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto area di celle corrente. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Ottiene o imposta la colonna finale di quest'area.

### EndRow {#EndRow}
```
public int EndRow
```


Ottiene o imposta la riga finale di quest'area.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Ottiene o imposta la colonna iniziale di quest'area.

### StartRow {#StartRow}
```
public int StartRow
```


Ottiene o imposta la riga iniziale di quest'area.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Confronta due oggetti CellArea in base al loro angolo in alto a sinistra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - Se due angoli sono in righe diverse, confronta il loro indice di riga. Altrimenti confronta il loro indice di colonna. Se i due angoli sono uguali, verrà restituito 0.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Crea un'area di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | La colonna di inizio. |
| endRow | int | La riga finale. |
| endColumn | int | La colonna finale. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Crea un'area di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCellName | java.lang.String | La cella in alto a sinistra dell'intervallo. |
| endCellName | java.lang.String | La cella in basso a destra dell'intervallo. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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


Restituisce una stringa che rappresenta l'oggetto area di celle corrente.

**Returns:**
java.lang.String -
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

