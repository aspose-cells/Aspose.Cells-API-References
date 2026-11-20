---
title: "RowCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Raccoglie gli oggetti che rappresentano le righe individuali in un foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Raccoglie gli oggetti [Row](../../com.aspose.cells/row) che rappresentano le righe individuali in un foglio di lavoro.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clear()](#clear--) | Cancella tutte le righe e le celle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Ottiene un oggetto [Row](../../com.aspose.cells/row) dato l'indice di riga. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di righe in questa collezione. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Ottiene l'oggetto riga in base alla posizione nella lista. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ottiene un enumeratore che itera le righe attraverso questa collezione |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Ottiene un enumeratore che itera le righe attraverso questa collezione |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento riga all'indice (posizione) specificato in questa collezione. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le righe e le celle.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Ottiene un oggetto [Row](../../com.aspose.cells/row) dato l'indice di riga. L'oggetto Row dell'indice di riga specificato verrà istanziato se non esiste già.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Ottiene il numero di righe in questa collezione.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Ottiene l'oggetto riga in base alla posizione nella lista.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | La posizione. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene un enumeratore che itera le righe attraverso questa collezione

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - L'enumeratore di righe che attraverserà tutte le righe esistenti in questa collezione.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Ottiene un enumeratore che itera le righe attraverso questa collezione

**Remarks**

Se la collezione di righe viene modificata (tramite operazioni che possono causare l'instanziazione di una nuova Row o la rimozione di una Row esistente) durante l'attraversamento con l'enumeratore, dovrebbe essere usato un enumeratore sincronizzato invece di un enumeratore normale affinché l'attraversamento possa continuare dalla posizione subito successiva a quella attraversata dall'ultimo MoveNext(). Tuttavia, oltre al vantaggio che nessun elemento venga saltato o attraversato più volte, lo svantaggio dell'enumeratore sincronizzato è che le prestazioni saranno leggermente degradate rispetto a un enumeratore normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| invertito | boolean | se enumerare le righe in ordine invertito |
| sincronizzato | boolean | se l'enumeratore restituito deve controllare la modifica della collezione di righe e rimanere sincronizzato con essa. |

**Returns:**
java.util.Iterator - L'enumeratore di righe che attraverserà tutte le righe esistenti in questa collezione.
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


Rimuove l'elemento riga all'indice (posizione) specificato in questa collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | indice basato su zero (posizione, non [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) dell'elemento riga esistente in questa collezione. |

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

