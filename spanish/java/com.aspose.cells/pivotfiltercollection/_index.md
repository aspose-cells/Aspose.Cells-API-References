---
title: "PivotFilterCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una colección de todos los PivotFilters."
type: docs
url: /es/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Representa una colección de todos los PivotFilters.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Agrega un objeto PivotFilter al tipo específico |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtra por configuración de fecha del campo pivot de fila o columna. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filtra por leyendas del campo pivot de fila o columna. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filtra por valores del campo pivot de datos. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filtra por valores del campo pivot de datos. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Borra PivotFilter del PivotField específico |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el objeto pivotfilter en el índice específico. |
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
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Agrega un objeto PivotFilter al tipo específico

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice los métodos PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() y AddDateFilter(). Este método será eliminado 12 meses después, a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | el índice del PivotField |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). el tipo de PivotFilter |

**Returns:**
int - el índice del objeto PivotFilter en esta PivotFilterCollection.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Filtra por configuración de fecha del campo pivot de fila o columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | int | El índice del campo en la fuente. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | La etiqueta de fecha de la condición de filtro |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | La etiqueta de fecha límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Filtra por leyendas del campo pivot de fila o columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | int | El índice del campo en la fuente. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| label1 | java.lang.String | La etiqueta de la condición de filtro |
| label2 | java.lang.String | La etiqueta límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtra por valores del campo pivot de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | int | El índice del campo en la fuente. |
| valueFieldIndex | int | El índice del campo de datos en la región de datos. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. Solo puede ser Count,Sum y Percent. |
| isTop | boolean | Indica si el filtro es de arriba o de abajo |
| itemCount | int | El recuento de elementos |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Filtra por valores del campo pivot de datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseFieldIndex | int | El índice del campo en la fuente. |
| valueFieldIndex | int | El índice del campo de valor en la región de valores. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). El tipo de filtrado de datos. |
| value1 | double | El valor de la condición de filtro |
| value2 | double | El valor límite superior de la condición de filtro entre |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Borra PivotFilter del PivotField específico

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | int | el índice del PivotField |

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
public PivotFilter get(int index)
```


Obtiene el objeto pivotfilter en el índice específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

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
| índice | int | El índice basado en cero del elemento a eliminar. |

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

