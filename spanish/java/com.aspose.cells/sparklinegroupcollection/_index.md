---
title: "SparklineGroupCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/sparklinegroupcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineGroupCollection extends CollectionBase
```

Encapsula una colección de objetos [SparklineGroup](../../com.aspose.cells/sparklinegroup).

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int type)](#add-int-) | Añade un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con un [Sparkline](../../com.aspose.cells/sparkline) a la colección. |
| [add(int type, String dataRange, boolean isVertical, CellArea locationRange)](#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-) | Añade un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con algunos [Sparkline](../../com.aspose.cells/sparkline) a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [clearSparklineGroups(CellArea cellArea)](#clearSparklineGroups-com.aspose.cells.CellArea-) | Limpia los grupos de sparkline que se superponen a un área de celdas. |
| [clearSparklines(CellArea cellArea)](#clearSparklines-com.aspose.cells.CellArea-) | Limpia los sparklines que están dentro de un área de celdas. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [SparklineGroup](../../com.aspose.cells/sparklinegroup) en el índice especificado. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


Añade un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con un [Sparkline](../../com.aspose.cells/sparkline) a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Especifica el tipo del grupo Sparkline. |

**Returns:**
int - índice del objeto [SparklineGroup](../../com.aspose.cells/sparklinegroup).
### add(int type, String dataRange, boolean isVertical, CellArea locationRange) {#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public int add(int type, String dataRange, boolean isVertical, CellArea locationRange)
```


Añade un [SparklineGroup](../../com.aspose.cells/sparklinegroup) con algunos [Sparkline](../../com.aspose.cells/sparkline) a la colección.

**Remarks**

Este método también creará sparklines. Si  es verdadero, el número de filas en dataRange y locationRange debe ser el mismo. Si  es falso, el número de columnas en dataRange y locationRange debe ser el mismo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Especifica el tipo del grupo Sparkline. |
| dataRange | java.lang.String | Especifica el rango de datos del grupo sparkline. |
| isVertical | boolean | Especifica si se deben trazar los sparklines del rango de datos por fila o por columna. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Especifica dónde se colocarán las sparklines. |

**Returns:**
int - índice del objeto [SparklineGroup](../../com.aspose.cells/sparklinegroup).
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


Elimina todos los objetos de la instancia de CollectionBase.

### clearSparklineGroups(CellArea cellArea) {#clearSparklineGroups-com.aspose.cells.CellArea-}
```
public void clearSparklineGroups(CellArea cellArea)
```


Limpia los grupos de sparkline que se superponen a un área de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Especifica el área de celdas |

### clearSparklines(CellArea cellArea) {#clearSparklines-com.aspose.cells.CellArea-}
```
public void clearSparklines(CellArea cellArea)
```


Limpia los sparklines que están dentro de un área de celdas.

**Remarks**

[SparklineGroup](../../com.aspose.cells/sparklinegroup) will be removed too if it does not contains any [Sparkline](../../com.aspose.cells/sparkline).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Especifica el área de celdas |

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
public SparklineGroup get(int index)
```


Obtiene el elemento [SparklineGroup](../../com.aspose.cells/sparklinegroup) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[SparklineGroup](../../com.aspose.cells/sparklinegroup) - The element at the specified index.
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

