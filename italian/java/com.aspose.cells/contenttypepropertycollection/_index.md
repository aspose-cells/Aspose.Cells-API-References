---
title: "ContentTypePropertyCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Una collezione di oggetti che rappresentano informazioni aggiuntive."
type: docs
url: /it/java/com.aspose.cells/contenttypepropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ContentTypePropertyCollection extends CollectionBase
```

Una collezione di oggetti [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) che rappresentano informazioni aggiuntive.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Add a new property.
          workbook.getContentTypeProperties().add("Admin", "Aspose", "text");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Aggiunge informazioni sulla proprietà del tipo di contenuto. |
| [add(String name, String value, String type)](#add-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge informazioni sulla proprietà del tipo di contenuto. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene la proprietà del tipo di contenuto tramite l'indice specifico. |
| [get(String name)](#get-java.lang.String-) | Ottiene la proprietà del tipo di contenuto tramite il nome della proprietà. |
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
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public int add(String name, String value)
```


Aggiunge informazioni sulla proprietà del tipo di contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà del tipo di contenuto. |
| valore | java.lang.String | Il valore della proprietà del tipo di contenuto. |

**Returns:**
int
### add(String name, String value, String type) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String name, String value, String type)
```


Aggiunge informazioni sulla proprietà del tipo di contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà del tipo di contenuto. |
| valore | java.lang.String | Il valore della proprietà del tipo di contenuto. |
| tipo | java.lang.String | Il tipo della proprietà del tipo di contenuto. |

**Returns:**
int
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
public ContentTypeProperty get(int index)
```


Ottiene la proprietà del tipo di contenuto tramite l'indice specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
### get(String name) {#get-java.lang.String-}
```
public ContentTypeProperty get(String name)
```


Ottiene la proprietà del tipo di contenuto tramite il nome della proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |

**Returns:**
[ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) - The content type property
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

