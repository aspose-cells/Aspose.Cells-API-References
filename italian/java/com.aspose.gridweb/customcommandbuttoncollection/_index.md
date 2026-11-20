---
title: "CustomCommandButtonCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la collezione di CustomCommandButton."
type: docs
url: /it/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Rappresenta la collezione di CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Aggiungi un oggetto pulsante di comando personalizzato alla collezione. |
| [clear()](#clear--) | Cancella la collezione. |
| [contains(Object value)](#contains-java.lang.Object-) | Indica se l'oggetto pulsante di comando personalizzato è nella collezione. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Copia la collezione in un array. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene un oggetto pulsante di comando personalizzato all'indice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il conteggio della collezione. |
| [getSyncRoot()](#getSyncRoot--) | Utilizzato solo internamente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Ottiene l'indice del pulsante. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserisce un pulsante all'indice. |
| [isFixedSize()](#isFixedSize--) | Utilizzato solo internamente. |
| [isReadOnly()](#isReadOnly--) | Utilizzato solo internamente. |
| [isSynchronized()](#isSynchronized--) | Utilizzato solo internamente. |
| [iterator()](#iterator--) | Ottiene un oggetto IEnumerator della collezione. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Rimuove l'oggetto pulsante di comando personalizzato. |
| [removeAt(int index)](#removeAt-int-) | Rimuove all'indice. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Aggiungi un oggetto pulsante di comando personalizzato alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | L'oggetto pulsante di comando personalizzato. |

**Returns:**
int - L'indice.
### clear() {#clear--}
```
public void clear()
```


Cancella la collezione.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Indica se l'oggetto pulsante di comando personalizzato è nella collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | Indica se l'oggetto pulsante di comando personalizzato è nella collezione. |

**Returns:**
boolean - vero o falso.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Copia la collezione in un array.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | java.lang.Object[] | L'array. |
| indice | int | L'indice di partenza dell'array. |

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
public CustomCommandButton get(int index)
```


Ottiene un oggetto pulsante di comando personalizzato all'indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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


Ottiene il conteggio della collezione.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Utilizzato solo internamente.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


Ottiene l'indice del pulsante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | L'oggetto pulsante. |

**Returns:**
int - L'indice.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Inserisce un pulsante all'indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice. |
| valore | java.lang.Object | L'oggetto CustomCommandButton. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Utilizzato solo internamente.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Utilizzato solo internamente.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Utilizzato solo internamente.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene un oggetto IEnumerator della collezione.

**Returns:**
java.util.Iterator - L'oggetto IEnumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


Rimuove l'oggetto pulsante di comando personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | L'oggetto pulsante di comando personalizzato. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove all'indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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

