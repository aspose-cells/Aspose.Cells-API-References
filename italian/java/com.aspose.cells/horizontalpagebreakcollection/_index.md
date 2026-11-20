---
title: "HorizontalPageBreakCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Incapsula una collezione di oggetti [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int row)](#add-int-) | Aggiunge un'interruzione di pagina orizzontale alla collezione. |
| [add(int row, int column)](#add-int-int-) | Aggiunge un'interruzione di pagina orizzontale alla collezione. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Aggiunge un'interruzione di pagina orizzontale alla collezione. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Aggiunge un'interruzione di pagina orizzontale alla collezione. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) all'indice specificato. |
| [get(String cellName)](#get-java.lang.String-) | Ottiene l'elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) con il nome di cella specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento HPageBreak con un nome specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Aggiunge un'interruzione di pagina orizzontale alla collezione.

**Remarks**

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga della cella, a base zero. |

**Returns:**
int - indice dell'oggetto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Aggiunge un'interruzione di pagina orizzontale alla collezione.

**Remarks**

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga della cella, a base zero. |
| colonna | int | Indice della colonna della cella, a base zero. |

**Returns:**
int - indice dell'oggetto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Aggiunge un'interruzione di pagina orizzontale alla collezione.

**Remarks**

Questo metodo è usato per aggiungere un'interruzione di pagina orizzontale all'interno di un'area di stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga, a base zero. |
| startColumn | int | Indice della colonna di partenza, a base zero. |
| endColumn | int | Indice della colonna finale, a base zero. |

**Returns:**
int - indice dell'oggetto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Aggiunge un'interruzione di pagina orizzontale alla collezione.

**Remarks**

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |

**Returns:**
int - indice dell'oggetto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
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
public HorizontalPageBreak get(int index)
```


Ottiene l'elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Ottiene l'elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) con il nome di cella specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuove l'elemento HPageBreak con un nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice dell'elemento, a base zero. |

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

