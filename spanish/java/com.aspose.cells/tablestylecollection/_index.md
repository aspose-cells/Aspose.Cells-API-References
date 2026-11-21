---
title: "TableStyleCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todos los estilos de tabla personalizados."
type: docs
url: /es/java/com.aspose.cells/tablestylecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleCollection extends CollectionBase
```

Representa todos los estilos de tabla personalizados.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [addPivotTableStyle(String name)](#addPivotTableStyle-java.lang.String-) | Agrega un estilo de tabla dinámica personalizado. |
| [addTableStyle(String name)](#addTableStyle-java.lang.String-) | Agrega un estilo de tabla personalizado. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el estilo de tabla por el índice. |
| [get(String name)](#get-java.lang.String-) | Obtiene el estilo de tabla por el nombre. |
| [getBuiltinTableStyle(int type)](#getBuiltinTableStyle-int-) | Obtiene el estilo de tabla incorporado |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--) | Obtiene el nombre del estilo predeterminado de la tabla dinámica. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--) | Obtiene el nombre del estilo predeterminado de la tabla. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [setDefaultPivotStyleName(String value)](#setDefaultPivotStyleName-java.lang.String-) | Establece el nombre del estilo predeterminado de la tabla dinámica. |
| [setDefaultTableStyleName(String value)](#setDefaultTableStyleName-java.lang.String-) | Establece el nombre del estilo predeterminado de la tabla. |
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
### addPivotTableStyle(String name) {#addPivotTableStyle-java.lang.String-}
```
public int addPivotTableStyle(String name)
```


Agrega un estilo de tabla dinámica personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del estilo de la tabla dinámica. |

**Returns:**
int - El índice del estilo de la tabla dinámica.
### addTableStyle(String name) {#addTableStyle-java.lang.String-}
```
public int addTableStyle(String name)
```


Agrega un estilo de tabla personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del estilo de tabla. |

**Returns:**
int - El índice del estilo de tabla.
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
public TableStyle get(int index)
```


Obtiene el estilo de tabla por el índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | La posición del estilo de tabla en la lista. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### get(String name) {#get-java.lang.String-}
```
public TableStyle get(String name)
```


Obtiene el estilo de tabla por el nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del estilo de tabla. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### getBuiltinTableStyle(int type) {#getBuiltinTableStyle-int-}
```
public TableStyle getBuiltinTableStyle(int type)
```


Obtiene el estilo de tabla incorporado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [TableStyleType](../../com.aspose.cells/tablestyletype). El tipo de estilo de tabla incorporado. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - 
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
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```
public String getDefaultPivotStyleName()
```


Obtiene el nombre del estilo predeterminado de la tabla dinámica.

**Returns:**
java.lang.String
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```
public String getDefaultTableStyleName()
```


Obtiene el nombre del estilo predeterminado de la tabla.

**Returns:**
java.lang.String
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

### setDefaultPivotStyleName(String value) {#setDefaultPivotStyleName-java.lang.String-}
```
public void setDefaultPivotStyleName(String value)
```


Establece el nombre del estilo predeterminado de la tabla dinámica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDefaultTableStyleName(String value) {#setDefaultTableStyleName-java.lang.String-}
```
public void setDefaultTableStyleName(String value)
```


Establece el nombre del estilo predeterminado de la tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

