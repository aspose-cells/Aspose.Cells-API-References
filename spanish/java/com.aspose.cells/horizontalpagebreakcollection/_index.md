---
title: "HorizontalPageBreakCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Encapsula una colección de objetos [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int row)](#add-int-) | Agrega un salto de página horizontal a la colección. |
| [add(int row, int column)](#add-int-int-) | Agrega un salto de página horizontal a la colección. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Agrega un salto de página horizontal a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Agrega un salto de página horizontal a la colección. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) en el índice especificado. |
| [get(String cellName)](#get-java.lang.String-) | Obtiene el elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) con el nombre de celda especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento HPageBreak con un nombre especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Agrega un salto de página horizontal a la colección.

**Remarks**

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila de celda, basado en cero. |

**Returns:**
int - índice del objeto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Agrega un salto de página horizontal a la colección.

**Remarks**

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila de celda, basado en cero. |
| columna | int | Índice de columna de celda, basado en cero. |

**Returns:**
int - índice del objeto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Agrega un salto de página horizontal a la colección.

**Remarks**

Este método se usa para agregar un salto de página horizontal dentro de un área de impresión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | Índice de fila, basado en cero. |
| startColumn | int | Índice de columna inicial, basado en cero. |
| endColumn | int | Índice de columna final, basado en cero. |

**Returns:**
int - índice del objeto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Agrega un salto de página horizontal a la colección.

**Remarks**

El salto de página se agrega en la esquina superior izquierda de la celda. Por favor, establezca un salto de página horizontal y un salto de página vertical simultáneamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de celda. |

**Returns:**
int - índice del objeto [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

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
public HorizontalPageBreak get(int index)
```


Obtiene el elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Obtiene el elemento [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) con el nombre de celda especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de celda. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


Elimina el elemento HPageBreak con un nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | Índice de elemento, basado en cero. |

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

