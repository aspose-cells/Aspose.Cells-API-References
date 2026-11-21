---
title: "SlicerCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica la colección de todos los objetos Slicer en la hoja de cálculo especificada."
type: docs
url: /es/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Especifica la colección de todos los objetos Slicer en la hoja de cálculo especificada.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Agrega un nuevo Segmentador usando ListObjet como fuente de datos |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Agrega un nuevo Segmentador usando ListObjet como fuente de datos |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Agrega un nuevo Segmentador usando ListObjet como fuente de datos |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Agrega un nuevo Segmentador usando PivotTable como fuente de datos |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Borra todos los Segmentadores. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el Segmentador por índice. |
| [get(String name)](#get-java.lang.String-) | Obtiene el Segmentador por el nombre del segmentador. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Elimina el Segmentador especificado |
| [removeAt(int index)](#removeAt-int-) | Elimina el Segmentador en el índice especificado |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Agrega un nuevo Segmentador usando ListObjet como fuente de datos

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject objeto |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn en ListObject.ListColumns |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango del Segmentador. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango del Segmentador. |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Agrega un nuevo Segmentador usando ListObjet como fuente de datos

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject objeto |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn en ListObject.ListColumns |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango del Segmentador. |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Agrega un nuevo Segmentador usando ListObjet como fuente de datos

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject objeto |
| índice | int | El índice de ListColumn en ListObject.ListColumns |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango del Segmentador. |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango del Segmentador. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango del Segmentador. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | El PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango del Segmentador. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango del Segmentador. |
| baseFieldIndex | int | El índice de PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| fila | int | Índice de fila de la celda en la esquina superior izquierda del rango del Segmentador. |
| columna | int | Índice de columna de la celda en la esquina superior izquierda del rango del Segmentador. |
| baseFieldName | java.lang.String | El nombre de PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango del Segmentador. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | El PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango del Segmentador. |
| baseFieldIndex | int | El índice de PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Agrega un nuevo Segmentador usando PivotTable como fuente de datos

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable objeto |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango del Segmentador. |
| baseFieldName | java.lang.String | El nombre de PivotField en PivotTable.BaseFields |

**Returns:**
int - El nuevo índice del Segmentador añadido
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


Borra todos los Segmentadores.

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
public Slicer get(int index)
```


Obtiene el Segmentador por índice.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Obtiene el Segmentador por el nombre del segmentador.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Elimina el Segmentador especificado

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | El objeto Slicer |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el Segmentador en el índice especificado

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de posición en la colección Slicer |

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

