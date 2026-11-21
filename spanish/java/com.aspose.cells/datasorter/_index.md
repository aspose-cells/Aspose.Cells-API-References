---
title: "DataSorter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Descripción resumida para DataSorter."
type: docs
url: /es/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Descripción resumida para DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Agrega clave de ordenación por color. |
| [addKey(int key, int order)](#addKey-int-int-) | Agrega el índice de columna ordenada y el orden de clasificación. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada. |
| [clear()](#clear--) | Borrar todas las configuraciones. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Obtiene si distingue mayúsculas y minúsculas al comparar cadenas. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [getKey2()](#getKey2--) | Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [getKey3()](#getKey3--) | Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [getKeys()](#getKeys--) | Obtiene la lista de claves del clasificador de datos. |
| [getOrder1()](#getOrder1--) | Representa el orden de clasificación de la primera clave. |
| [getOrder2()](#getOrder2--) | Representa el orden de clasificación de la segunda clave. |
| [getOrder3()](#getOrder3--) | Representa el orden de clasificación de la tercera clave. |
| [getSortAsNumber()](#getSortAsNumber--) | Indica si se ordena cualquier cosa que parezca un número. |
| [getSortLeftToRight()](#getSortLeftToRight--) | Verdadero significa que la orientación de ordenación es de izquierda a derecha. |
| [hasHeaders()](#hasHeaders--) | Representa si el rango tiene encabezados. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Establece si distingue mayúsculas y minúsculas al comparar cadenas. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Representa si el rango tiene encabezados. |
| [setKey1(int value)](#setKey1-int-) | Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Representa el orden de clasificación de la primera clave. |
| [setOrder2(int value)](#setOrder2-int-) | Representa el orden de clasificación de la segunda clave. |
| [setOrder3(int value)](#setOrder3-int-) | Representa el orden de clasificación de la tercera clave. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Indica si se ordena cualquier cosa que parezca un número. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | Verdadero significa que la orientación de ordenación es de izquierda a derecha. |
| [sort()](#sort--) | Ordena los datos en el rango. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Ordenar los datos del área. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Ordena los datos del área. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Agrega clave de ordenación por color.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | int | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). El tipo de valor de color ordenado. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). El orden de clasificación. |
| color | [Color](../../com.aspose.cells/color) | El color de ordenación personalizado. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Agrega el índice de columna ordenada y el orden de clasificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | int | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). El orden de clasificación |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada.

**Remarks**

Si el tipo es SortOnType.CellColor o SortOnType.FontColor, customList es Color.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | int | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). El tipo de valor ordenado. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). El orden de clasificación. |
| customList | java.lang.Object | La lista de ordenación personalizada. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | int | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). El orden de clasificación. |
| customList | java.lang.String | La lista de ordenación personalizada. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Agrega el índice de columna ordenada y el orden de clasificación con una lista de ordenación personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | int | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). El orden de clasificación. |
| customList | java.lang.String[] | La lista de ordenación personalizada. |

### clear() {#clear--}
```
public void clear()
```


Borrar todas las configuraciones.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Obtiene si distingue mayúsculas y minúsculas al comparar cadenas.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Obtiene la lista de claves del clasificador de datos.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Representa el orden de clasificación de la primera clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Representa el orden de clasificación de la segunda clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Representa el orden de clasificación de la tercera clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Indica si se ordena cualquier cosa que parezca un número.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True significa que la orientación de ordenación es de izquierda a derecha. False significa que la orientación de ordenación es de arriba a abajo. El valor predeterminado es false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Representa si el rango tiene encabezados.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Establece si distingue mayúsculas y minúsculas al comparar cadenas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Representa si el rango tiene encabezados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Representa el orden de clasificación de la primera clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Representa el orden de clasificación de la segunda clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Representa el orden de clasificación de la tercera clave.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Indica si se ordena cualquier cosa que parezca un número.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True significa que la orientación de ordenación es de izquierda a derecha. False significa que la orientación de ordenación es de arriba a abajo. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Ordena los datos en el rango.

**Returns:**
int[] - los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesitan mover filas/columnas con esta operación de ordenación, se devolverá null.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Ordenar los datos del área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Las celdas contienen el área de datos. |
| area | [CellArea](../../com.aspose.cells/cellarea) | El área necesaria para ordenar |

**Returns:**
int[] - los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesitan mover filas/columnas con esta operación de ordenación, se devolverá null.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Ordena los datos del área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Las celdas contienen el área de datos. |
| startRow | int | La fila inicial del área. |
| startColumn | int | La columna inicial del área. |
| endRow | int | La fila final del área. |
| endColumn | int | La columna final del área. |

**Returns:**
int[] - los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesitan mover filas/columnas con esta operación de ordenación, se devolverá null.
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

