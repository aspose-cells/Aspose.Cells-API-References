---
title: "GridHyperlinkCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Incapsula una raccolta di oggetti [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Aggiunge un collegamento ipertestuale a una cella specificata. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [clear()](#clear--) | Cancella tutti gli hyperlink. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Restituisce la dimensione dell'enumeratore |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Ottiene l'oggetto Hyperlink della cella. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Ottiene l'oggetto Hyperlink della cella. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Rimuove il collegamento ipertestuale nell'area specificata. |
| [removeAt(int index)](#removeAt-int-) | Rimuove il collegamento ipertestuale all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga dell'intervallo di hyperlink. |
| firstColumn | int | Prima colonna dell'intervallo di hyperlink. |
| totalRows | int | Numero di righe in questo intervallo di hyperlink. |
| totalColumns | int | Numero di colonne di questo intervallo di hyperlink. |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |

**Returns:**
int - indice dell'oggetto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |
| totalRows | int | Numero di righe in questo intervallo di hyperlink. |
| totalColumns | int | Numero di colonne di questo intervallo di hyperlink. |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |

**Returns:**
int - indice dell'oggetto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Aggiunge un collegamento ipertestuale a una cella specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |

**Returns:**
int - indice dell'oggetto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCellName | java.lang.String | La cella in alto a sinistra dell'intervallo. |
| endCellName | java.lang.String | La cella in basso a destra dell'intervallo. |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |
| textToDisplay | java.lang.String | Il testo da visualizzare per il collegamento ipertestuale specificato. |
| screenTip | java.lang.String | Il testo screenTip per il collegamento ipertestuale specificato. |

**Returns:**
int - indice dell'oggetto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### clear() {#clear--}
```
public void clear()
```


Cancella tutti gli hyperlink.

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
### get(int index) {#get-int-}
```
public GridHyperlink get(int index)
```


Ottiene l'elemento [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Restituisce la dimensione dell'enumeratore

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Ottiene l'oggetto Hyperlink della cella. Se la cella non ha un Hyperlink, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | L'oggetto GridCell. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Ottiene l'oggetto Hyperlink della cella. Se la cella non ha un Hyperlink, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | La riga della cella. |
| colonna | int | La colonna della cella. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Rimuove il collegamento ipertestuale nell'area specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area che contiene il collegamento ipertestuale. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove il collegamento ipertestuale all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

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

