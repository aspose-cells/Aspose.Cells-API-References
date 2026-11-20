---
title: "DataSorter"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrizione riepilogativa per DataSorter."
type: docs
url: /it/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Descrizione riepilogativa per DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Aggiunge la chiave di ordinamento colore. |
| [addKey(int key, int order)](#addKey-int-int-) | Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [clear()](#clear--) | Cancella tutte le impostazioni. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Ottiene se è sensibile al maiuscolo/minuscolo durante il confronto delle stringhe. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [getKey2()](#getKey2--) | Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [getKey3()](#getKey3--) | Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [getKeys()](#getKeys--) | Ottiene l'elenco delle chiavi del DataSorter. |
| [getOrder1()](#getOrder1--) | Rappresenta l'ordine di ordinamento della prima chiave. |
| [getOrder2()](#getOrder2--) | Rappresenta l'ordine di ordinamento della seconda chiave. |
| [getOrder3()](#getOrder3--) | Rappresenta l'ordine di ordinamento della terza chiave. |
| [getSortAsNumber()](#getSortAsNumber--) | Indica se ordinare tutto ciò che sembra un numero. |
| [getSortLeftToRight()](#getSortLeftToRight--) | Vero significa che l'orientamento dell'ordinamento è da sinistra a destra. |
| [hasHeaders()](#hasHeaders--) | Rappresenta se l'intervallo ha intestazioni. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Imposta se è sensibile al maiuscolo/minuscolo durante il confronto delle stringhe. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Rappresenta se l'intervallo ha intestazioni. |
| [setKey1(int value)](#setKey1-int-) | Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Rappresenta l'ordine di ordinamento della prima chiave. |
| [setOrder2(int value)](#setOrder2-int-) | Rappresenta l'ordine di ordinamento della seconda chiave. |
| [setOrder3(int value)](#setOrder3-int-) | Rappresenta l'ordine di ordinamento della terza chiave. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Indica se ordinare tutto ciò che sembra un numero. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | Vero significa che l'orientamento dell'ordinamento è da sinistra a destra. |
| [sort()](#sort--) | Ordina i dati nell'intervallo. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Ordina i dati dell'area. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Ordina i dati dell'area. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Aggiunge la chiave di ordinamento colore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | int | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Il tipo di valore di colore ordinato. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordine di ordinamento. |
| color | [Color](../../com.aspose.cells/color) | Il colore di ordinamento personalizzato. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | int | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordine di ordinamento |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

**Remarks**

Se il tipo è SortOnType.CellColor o SortOnType.FontColor, la customList è Color.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | int | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Il tipo di valore ordinato. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordine di ordinamento. |
| customList | java.lang.Object | L'elenco di ordinamento personalizzato. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | int | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordine di ordinamento. |
| customList | java.lang.String | L'elenco di ordinamento personalizzato. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | int | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordine di ordinamento. |
| customList | java.lang.String[] | L'elenco di ordinamento personalizzato. |

### clear() {#clear--}
```
public void clear()
```


Cancella tutte le impostazioni.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Ottiene se è sensibile al maiuscolo/minuscolo durante il confronto delle stringhe.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Ottiene l'elenco delle chiavi del DataSorter.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Rappresenta l'ordine di ordinamento della prima chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Rappresenta l'ordine di ordinamento della seconda chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Rappresenta l'ordine di ordinamento della terza chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Indica se ordinare tutto ciò che sembra un numero.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True indica che l'orientamento dell'ordinamento è da sinistra a destra. False indica che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Rappresenta se l'intervallo ha intestazioni.

**Returns:**
boolean
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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Imposta se è sensibile al maiuscolo/minuscolo durante il confronto delle stringhe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Rappresenta se l'intervallo ha intestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Rappresenta l'ordine di ordinamento della prima chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Rappresenta l'ordine di ordinamento della seconda chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Rappresenta l'ordine di ordinamento della terza chiave.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Indica se ordinare tutto ciò che sembra un numero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True indica che l'orientamento dell'ordinamento è da sinistra a destra. False indica che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Ordina i dati nell'intervallo.

**Returns:**
int[] - gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Ordina i dati dell'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Le celle contengono l'area dei dati. |
| area | [CellArea](../../com.aspose.cells/cellarea) | L'area da ordinare |

**Returns:**
int[] - gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Ordina i dati dell'area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Le celle contengono l'area dei dati. |
| startRow | int | La riga iniziale dell'area. |
| startColumn | int | La colonna iniziale dell'area. |
| endRow | int | La riga finale dell'area. |
| endColumn | int | La colonna finale dell'area. |

**Returns:**
int[] - gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.
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

