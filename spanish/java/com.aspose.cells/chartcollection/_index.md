---
title: "ChartCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

Encapsula una colección de objetos [Chart](../../com.aspose.cells/chart).

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Agrega un gráfico con una plantilla predefinida. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | Agrega un gráfico a la colección. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Agrega un gráfico a la colección. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Agrega un gráfico a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Agrega un gráfico a la colección. |
| [clear()](#clear--) | Elimina todos los gráficos. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [Chart](../../com.aspose.cells/chart) en el índice especificado. |
| [get(String name)](#get-java.lang.String-) | Obtiene el gráfico por su nombre. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Elimina el gráfico específico. |
| [removeAt(int index)](#removeAt-int-) | Elimina un gráfico en el índice específico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Agrega un gráfico con una plantilla predefinida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | byte[] | Los datos del archivo de plantilla de gráfico (.crtx). |
| dataRange | java.lang.String | Especifica el rango de datos del gráfico |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| rightRow | int | Índice de fila inferior derecha |
| bottomColumn | int | Índice de columna inferior derecha |

**Returns:**
int - índice del objeto [Chart](../../com.aspose.cells/chart).
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Agrega un gráfico a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Tipo de gráfico |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |

**Returns:**
int - índice del objeto [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Agrega un gráfico a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Tipo de gráfico |
| dataRange | java.lang.String | Especifica el rango de datos del gráfico |
| isVertical | boolean | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| rightRow | int | Índice de fila inferior derecha |
| bottomColumn | int | Índice de columna inferior derecha |

**Returns:**
int - índice del objeto [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Agrega un gráfico a la colección.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-). Esta propiedad será eliminada 12 meses después desde mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Tipo de gráfico |
| dataRange | java.lang.String | Especifica el rango de datos del gráfico |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| rightRow | int | Índice de fila inferior derecha |
| bottomColumn | int | Índice de columna inferior derecha |

**Returns:**
int - índice del objeto [Chart](../../com.aspose.cells/chart).
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
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


Agrega un gráfico a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Tipo de gráfico |
| izquierda | int | El desplazamiento x a la esquina |
| superior | int | El desplazamiento y a la esquina |
| ancho | int | El ancho del gráfico |
| altura | int | La altura del gráfico |

**Returns:**
int - índice del objeto [Chart](../../com.aspose.cells/chart).
### clear() {#clear--}
```
public void clear()
```


Elimina todos los gráficos.

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
public Chart get(int index)
```


Obtiene el elemento [Chart](../../com.aspose.cells/chart) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


Obtiene el gráfico por su nombre.

**Remarks**

El nombre predeterminado del gráfico es nulo. Por lo tanto, debe establecer explícitamente el nombre del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del gráfico. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


Elimina el gráfico específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina un gráfico en el índice específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice del gráfico. |

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

