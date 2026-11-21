---
title: "NameCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una colección de todos los objetos en la hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Representa una colección de todos los objetos [Name](../../com.aspose.cells/name) en la hoja de cálculo.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String text)](#add-java.lang.String-) | Define un nuevo nombre. |
| [clear()](#clear--) | Elimina todos los nombres definidos que no están referenciados por las fórmulas y la fuente de datos. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Obtiene todos los nombres definidos por alcance. |
| [get(int index)](#get-int-) | Obtiene el elemento [Name](../../com.aspose.cells/name) en el índice especificado. |
| [get(String text)](#get-java.lang.String-) | Obtiene el elemento [Name](../../com.aspose.cells/name) con el nombre especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Elimina el nombre. |
| [remove(String[] names)](#remove-java.lang.String---) | Elimina una matriz de nombres. |
| [removeAt(int index)](#removeAt-int-) | Elimina el nombre en el índice específico. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Elimina los nombres definidos duplicados. |
| [sort()](#sort--) | Ordena los nombres definidos. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Define un nuevo nombre.

**Remarks**

El nombre no puede incluir espacios y no puede parecer referencias de celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | El texto a usar como nombre. |

**Returns:**
int - índice del objeto [Name](../../com.aspose.cells/name).
### clear() {#clear--}
```
public void clear()
```


Elimina todos los nombres definidos que no están referenciados por las fórmulas y la fuente de datos. Si el nombre definido está referenciado, solo establecemos Name.ReferTo como nulo y los ocultamos.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Obtiene todos los nombres definidos por alcance.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). El tipo de alcance. |
| sheetIndex | int | El índice de la hoja. Solo afecta cuando el tipo de alcance es [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Obtiene el elemento [Name](../../com.aspose.cells/name) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Obtiene el elemento [Name](../../com.aspose.cells/name) con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | Texto del nombre. |

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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
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


Elimina el nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | El texto del nombre. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Elimina una matriz de nombres.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| names | java.lang.String[] | El texto de los nombres. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el nombre en el índice específico.

**Remarks**

Por favor, asegúrese de que el nombre no sea referenciado por otras fórmulas antes de llamar al método. Y si el nombre es referenciado, establecer Name.RefersTo como null es mejor.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | índice del Name que se eliminará. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Elimina los nombres definidos duplicados.

### sort() {#sort--}
```
public void sort()
```


Ordena los nombres definidos.

**Remarks**

Si crea una gran cantidad de rangos con nombre en el archivo Excel, llame a este método después de que se hayan creado todos los rangos con nombre y antes de guardar.

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

