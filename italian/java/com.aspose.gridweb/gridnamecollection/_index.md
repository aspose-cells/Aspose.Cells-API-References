---
title: "GridNameCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Incapsula una collezione di oggetti [GridName](../../com.aspose.gridweb/gridname).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Definisce un nuovo nome nel foglio specificato. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Definisce un nuovo nome globale. |
| [clear()](#clear--) | Rimuove tutti i Nomi; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [GridName](../../com.aspose.gridweb/gridname) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Restituisce la dimensione dell'enumeratore |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Restituisce l'enumeratore delle righe |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Rimuove un array di nomi |
| [removeAt(int index)](#removeAt-int-) | Rimuove il nome all'indice specifico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Definisce un nuovo nome nel foglio specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | L'indice del foglio in cui il nome è applicato. |
| testo | java.lang.String | Testo del nome. Non può contenere il nome del foglio. |
| refersTo | java.lang.String | La formula a cui il nome è definito per fare riferimento. Deve contenere il nome del foglio, es. 'sheet hello!'A1:B2. |

**Returns:**
int - indice dell'oggetto Nome.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Definisce un nuovo nome globale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Testo del nome. Può contenere il nome del foglio. |
| refersTo | java.lang.String | La formula a cui il nome è definito per fare riferimento. Deve contenere un nome del foglio, es. 'sheet hello!'A1:B2. |

**Returns:**
int - indice dell'oggetto Nome.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti i Nomi;

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
public GridName get(int index)
```


Ottiene l'elemento [GridName](../../com.aspose.gridweb/gridname) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce l'enumeratore delle righe

**Returns:**
java.util.Iterator - L'enumeratore delle righe
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

Assicurati che il nome non sia referenziato da altre formule prima di chiamare il metodo. E se il nome è referenziato, imposta solo Name.RefersTo a null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

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

