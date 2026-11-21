---
title: "OleObjectCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa objetos OLE incrustados."
type: docs
url: /es/java/com.aspose.cells/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class OleObjectCollection extends CollectionBase
```

Representa objetos OLE incrustados.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData)](#add-int-int-int-int-byte---) | Agrega un OleObject a la colección. |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)](#add-int-int-int-int-byte---java.lang.String-) | Agrega un OleObject vinculado a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Eliminar todos los objetos OLE incrustados. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [OleObject](../../com.aspose.cells/oleobject) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width, byte[] imageData) {#add-int-int-int-int-byte---}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```


Agrega un OleObject a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| altura | int | Altura del oleObject, en unidades de píxel. |
| ancho | int | Ancho del oleObject, en unidades de píxel. |
| imageData | byte[] | Imagen del objeto ole como matriz de bytes. |

**Returns:**
int - índice del objeto [OleObject](../../com.aspose.cells/oleobject).
### add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile) {#add-int-int-int-int-byte---java.lang.String-}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)
```


Agrega un OleObject vinculado a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| altura | int | Altura del oleObject, en unidades de píxel. |
| ancho | int | Ancho del oleObject, en unidades de píxel. |
| imageData | byte[] | Imagen del objeto ole como matriz de bytes. |
| linkedFile | java.lang.String |  |

**Returns:**
int - índice del objeto [OleObject](../../com.aspose.cells/oleobject).
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
### clear() {#clear--}
```
public void clear()
```


Eliminar todos los objetos OLE incrustados.

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
### get(int index) {#get-int-}
```
public OleObject get(int index)
```


Obtiene el elemento [OleObject](../../com.aspose.cells/oleobject) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - The element at the specified index.
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice especificado. |

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

