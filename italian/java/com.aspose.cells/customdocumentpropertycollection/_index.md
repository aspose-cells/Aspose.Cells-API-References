---
title: "CustomDocumentPropertyCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Una raccolta di proprietà personalizzate del documento."
type: docs
url: /it/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

Una raccolta di proprietà personalizzate del documento.

**Remarks**

Ogni oggetto rappresenta una proprietà personalizzata di un documento contenitore.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crea una nuova proprietà personalizzata del documento di tipo dati **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | Crea una nuova proprietà personalizzata del documento di tipo dati **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | Crea una nuova proprietà personalizzata del documento che collega al contenuto. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [contains(String name)](#contains-java.lang.String-) | Restituisce true se una proprietà con il nome specificato esiste nella collezione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per indice. |
| [get(String name)](#get-java.lang.String-) | Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per il nome della proprietà. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Ottiene l'indice di una proprietà per nome. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Rimuove una proprietà con il nome specificato dalla collezione. |
| [removeAt(int index)](#removeAt-int-) | Rimuove una proprietà all'indice specificato. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto (usa il valore della cella dell'intervallo collegato per aggiornare il valore della proprietà personalizzata). |
| [updateLinkedRange()](#updateLinkedRange--) | Aggiorna tutti gli intervalli collegati alle proprietà personalizzate (usa il valore della proprietà personalizzata del documento per aggiornare il valore della cella dell'intervallo collegato). |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


Crea una nuova proprietà personalizzata del documento di tipo dati **PropertyType.Boolean**.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | boolean | Il valore della proprietà. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


Crea una nuova proprietà personalizzata del documento di tipo dati **PropertyType.DateTime**.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| value | [DateTime](../../com.aspose.cells/datetime) | Il valore della proprietà. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.Float**.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | double | Il valore della proprietà. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.Number**.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | int | Il valore della proprietà. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Crea una nuova proprietà personalizzata del documento del tipo di dati **PropertyType.String**.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | java.lang.String | Il valore della proprietà. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


Crea una nuova proprietà personalizzata del documento che collega al contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| origine | java.lang.String | L'origine della proprietà. Dovrebbe essere il nome dell'intervallo denominato. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Restituisce true se una proprietà con il nome specificato esiste nella collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

**Returns:**
boolean - True se la proprietà esiste nella collezione; false altrimenti.
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
public DocumentProperty get(int index)
```


Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | Indice basato su zero del [DocumentProperty](../../com.aspose.cells/documentproperty) da recuperare. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per il nome della proprietà.

**Remarks**

Restituisce null se una proprietà con il nome specificato non viene trovata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole, da recuperare. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Ottiene l'indice di una proprietà per nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

**Returns:**
int - L'indice basato su zero. Valore negativo se non trovato.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Rimuove una proprietà con il nome specificato dalla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove una proprietà all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto (usa il valore della cella dell'intervallo collegato per aggiornare il valore della proprietà personalizzata).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Aggiorna tutti gli intervalli collegati alle proprietà personalizzate (usa il valore della proprietà personalizzata del documento per aggiornare il valore della cella dell'intervallo collegato).

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

