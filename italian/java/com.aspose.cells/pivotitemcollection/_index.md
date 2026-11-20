---
title: "PivotItemCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutti gli oggetti nel PivotField."
type: docs
url: /it/java/com.aspose.cells/pivotitemcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotItemCollection extends CollectionBase
```

Rappresenta tutti gli oggetti [PivotItem](../../com.aspose.cells/pivotitem) nel PivotField.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [changeitemsOrder(int sourceIndex, int destIndex)](#changeitemsOrder-int-int-) | Modifica direttamente l'ordine dei due elementi. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'oggetto PivotItem all'indice specifico. |
| [get(String itemValue)](#get-java.lang.String-) | Ottiene il [PivotItem](../../com.aspose.cells/pivotitem) per nome specifico. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetail(boolean isHiddenDetail)](#hideAllDetail-boolean-) | Imposta se nascondere tutti i dettagli di tutti i PivotItem in un campo pivot. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [swapItem(int index1, int index2)](#swapItem-int-int-) | Scambia direttamente due elementi. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### changeitemsOrder(int sourceIndex, int destIndex) {#changeitemsOrder-int-int-}
```
public void changeitemsOrder(int sourceIndex, int destIndex)
```


Modifica direttamente l'ordine dei due elementi.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotItemCollection.SwapItem(). Questo metodo sarà rimosso tra 12 mesi a partire da luglio 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | int | L'indice corrente |
| destIndex | int | L'indice di destinazione |

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
public PivotItem get(int index)
```


Ottiene l'oggetto PivotItem all'indice specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
### get(String itemValue) {#get-java.lang.String-}
```
public PivotItem get(String itemValue)
```


Ottiene il [PivotItem](../../com.aspose.cells/pivotitem) per nome specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemValue | java.lang.String |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
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
### hideAllDetail(boolean isHiddenDetail) {#hideAllDetail-boolean-}
```
public void hideAllDetail(boolean isHiddenDetail)
```


Imposta se nascondere tutti i dettagli di tutti i PivotItem in un campo pivot. Cioè comprimere/espandere questo campo.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi PivotField.HideAllDetails() e ShowAllDetails() al suo posto. Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isHiddenDetail | boolean | Indica se nascondere il dettaglio del campo pivot. |

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


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

### swapItem(int index1, int index2) {#swapItem-int-int-}
```
public void swapItem(int index1, int index2)
```


Scambia direttamente due elementi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index1 | int |  |
| index2 | int |  |

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

