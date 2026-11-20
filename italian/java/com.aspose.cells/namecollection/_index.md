---
title: "NameCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una collezione di tutti gli oggetti nel foglio di calcolo."
type: docs
url: /it/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Rappresenta una collezione di tutti gli oggetti [Name](../../com.aspose.cells/name) nel foglio di calcolo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String text)](#add-java.lang.String-) | Definisce un nuovo nome. |
| [clear()](#clear--) | Rimuove tutti i nomi definiti che non sono referenziati dalle formule e dalla fonte dati. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Ottiene tutti i nomi definiti per ambito. |
| [get(int index)](#get-int-) | Ottiene l'elemento [Name](../../com.aspose.cells/name) all'indice specificato. |
| [get(String text)](#get-java.lang.String-) | Ottiene l'elemento [Name](../../com.aspose.cells/name) con il nome specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Rimuove il nome. |
| [remove(String[] names)](#remove-java.lang.String---) | Rimuove un array di nomi |
| [removeAt(int index)](#removeAt-int-) | Rimuove il nome all'indice specifico. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Rimuove i nomi definiti duplicati |
| [sort()](#sort--) | Ordina i nomi definiti. |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Definisce un nuovo nome.

**Remarks**

Il nome non può includere spazi e non può assomigliare a riferimenti di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo da utilizzare come nome. |

**Returns:**
int - indice dell'oggetto [Name](../../com.aspose.cells/name).
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti i nomi definiti che non sono referenziati dalle formule e dalla fonte dati. Se il nome definito è referenziato, impostiamo solo Name.ReferTo a null e lo nascondiamo.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Ottiene tutti i nomi definiti per ambito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Il tipo di ambito. |
| sheetIndex | int | L'indice del foglio. Ha effetto solo quando il tipo di ambito è [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Ottiene l'elemento [Name](../../com.aspose.cells/name) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Ottiene l'elemento [Name](../../com.aspose.cells/name) con il nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Testo del nome. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Rimuove il nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo del nome. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Rimuove un array di nomi

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomi | java.lang.String[] | Il testo dei nomi. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove il nome all'indice specifico.

**Remarks**

Assicurati che il nome non sia referenziato da altre formule prima di chiamare il metodo. E se il nome è referenziato, impostare Name.RefersTo a null è meglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | indice del Name da rimuovere. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Rimuove i nomi definiti duplicati

### sort() {#sort--}
```
public void sort()
```


Ordina i nomi definiti.

**Remarks**

Se crei un gran numero di intervalli denominati nel file Excel, chiama questo metodo dopo che tutti gli intervalli denominati sono stati creati e prima di salvare.

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

