---
title: "CustomCommandButtonCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la colección de CustomCommandButton."
type: docs
url: /es/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Representa la colección de CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Agregar un objeto de botón de comando personalizado a la colección. |
| [clear()](#clear--) | Limpia la colección. |
| [contains(Object value)](#contains-java.lang.Object-) | Indica si el objeto de botón de comando personalizado está en la colección. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Copia la colección a un arreglo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene un objeto de botón de comando personalizado en el índice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el recuento de la colección. |
| [getSyncRoot()](#getSyncRoot--) | Solo de uso interno. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Obtiene el índice del botón. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserta un botón en el índice. |
| [isFixedSize()](#isFixedSize--) | Solo de uso interno. |
| [isReadOnly()](#isReadOnly--) | Solo de uso interno. |
| [isSynchronized()](#isSynchronized--) | Solo de uso interno. |
| [iterator()](#iterator--) | Obtiene un objeto IEnumerator de la colección. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Elimina el objeto de botón de comando personalizado. |
| [removeAt(int index)](#removeAt-int-) | Elimina en el índice. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Agregar un objeto de botón de comando personalizado a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | El objeto de botón de comando personalizado. |

**Returns:**
int - El índice.
### clear() {#clear--}
```
public void clear()
```


Limpia la colección.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Indica si el objeto de botón de comando personalizado está en la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | Indica si el objeto de botón de comando personalizado está en la colección. |

**Returns:**
boolean - Verdadero o falso.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Copia la colección a un arreglo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arreglo | java.lang.Object[] | El arreglo. |
| índice | int | El índice inicial del arreglo. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public CustomCommandButton get(int index)
```


Obtiene un objeto de botón de comando personalizado en el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

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


Obtiene el recuento de la colección.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Solo de uso interno.

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


Obtiene el índice del botón.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | El objeto del botón. |

**Returns:**
int - El índice.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Inserta un botón en el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice. |
| valor | java.lang.Object | El objeto CustomCommandButton. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Solo de uso interno.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Solo de uso interno.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Solo de uso interno.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtiene un objeto IEnumerator de la colección.

**Returns:**
java.util.Iterator - El objeto IEnumerator.
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


Elimina el objeto de botón de comando personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | El objeto de botón de comando personalizado. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina en el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

