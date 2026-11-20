---
title: "GridPivotTableCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Incapsula una raccolta di oggetti [GridPivotTable](../../com.aspose.gridweb/gridpivottable).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches. |
| [clear()](#clear--) | Cancella tutte le PivotTable. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [GridPivotTable](../../com.aspose.gridweb/gridpivottable) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Restituisce la dimensione dell'enumeratore |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove la PivotTable all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Il foglio di lavoro di origine. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area nel foglio di lavoro di origine. |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheetname | java.lang.String | Il nome del foglio di lavoro di origine. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area nel foglio di lavoro di origine. |
| destRow | int | La riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| destCol | int | La colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheetname | java.lang.String | Il nome del foglio di lavoro di origine. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area nel foglio di lavoro di origine. |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Aggiunge una nuova cache di PivotTable a una raccolta PivotCaches.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della cache appena aggiunta.
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le PivotTable.

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
public GridPivotTable get(int index)
```


Ottiene l'elemento [GridPivotTable](../../com.aspose.gridweb/gridpivottable) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove la PivotTable all'indice specificato.

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

