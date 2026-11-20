---
title: "PivotFilterCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una collezione di tutti i PivotFilter."
type: docs
url: /it/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Rappresenta una collezione di tutti i PivotFilter.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Aggiunge un oggetto PivotFilter al tipo specifico |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtra per impostazione della data del campo pivot di riga o colonna. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filtra per didascalie del campo pivot di riga o colonna. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filtra per valori del campo pivot dei dati. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filtra per valori del campo pivot dei dati. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Cancella PivotFilter dal PivotField specifico |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'oggetto pivotfilter all'indice specifico. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Aggiunge un oggetto PivotFilter al tipo specifico

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() e AddDateFilter(). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | l'indice del PivotField |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). il tipo di PivotFilter |

**Returns:**
int - l'indice dell'oggetto PivotFilter in questa PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Filtra per impostazione della data del campo pivot di riga o colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | int | L'indice del campo nella sorgente. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | L'etichetta della data della condizione di filtro |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | L'etichetta della data limite superiore della condizione di filtro between |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Filtra per didascalie del campo pivot di riga o colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | int | L'indice del campo nella sorgente. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| label1 | java.lang.String | L'etichetta della condizione di filtro |
| label2 | java.lang.String | L'etichetta di limite superiore della condizione di filtro tra |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtra per valori del campo pivot dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | int | L'indice del campo nella sorgente. |
| valueFieldIndex | int | L'indice del campo dati nella regione dati. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. Può essere solo Count, Sum e Percent. |
| isTop | boolean | Indica se il filtro è dal superiore o dal inferiore |
| itemCount | int | Il numero di elementi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Filtra per valori del campo pivot dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | int | L'indice del campo nella sorgente. |
| valueFieldIndex | int | L'indice del campo valore nella regione valore. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| value1 | double | Il valore della condizione di filtro |
| value2 | double | Il valore di limite superiore della condizione di filtro tra |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Cancella PivotFilter dal PivotField specifico

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | l'indice del PivotField |

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
public PivotFilter get(int index)
```


Ottiene l'oggetto pivotfilter all'indice specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

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

