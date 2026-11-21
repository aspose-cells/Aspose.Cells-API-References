---
title: "GridHyperlinkCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Encapsula una colección de [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objetos.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Agrega un hipervínculo a una celda especificada. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [clear()](#clear--) | Elimina todos los hipervínculos. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el tamaño del enumerador |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Obtiene el objeto Hyperlink de la celda. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Obtiene el objeto Hyperlink de la celda. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Elimina el hipervínculo en el área especificada. |
| [removeAt(int index)](#removeAt-int-) | Elimina el hipervínculo en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Agrega un hipervínculo a una celda especificada o a un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | int | Primera fila del rango de hipervínculos. |
| firstColumn | int | Primera columna del rango de hipervínculos. |
| totalRows | int | Número de filas en este rango de hipervínculos. |
| totalColumns | int | Número de columnas de este rango de hipervínculos. |
| dirección | java.lang.String | Dirección del hipervínculo. |

**Returns:**
int - índice del objeto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Agrega un hipervínculo a una celda especificada o a un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de celda. |
| totalRows | int | Número de filas en este rango de hipervínculos. |
| totalColumns | int | Número de columnas de este rango de hipervínculos. |
| dirección | java.lang.String | Dirección del hipervínculo. |

**Returns:**
int - índice del objeto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Agrega un hipervínculo a una celda especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | java.lang.String | Nombre de celda. |
| dirección | java.lang.String | Dirección del hipervínculo. |

**Returns:**
int - índice del objeto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Agrega un hipervínculo a una celda especificada o a un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCellName | java.lang.String | La celda superior izquierda del rango. |
| endCellName | java.lang.String | La celda inferior derecha del rango. |
| dirección | java.lang.String | Dirección del hipervínculo. |
| textToDisplay | java.lang.String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | java.lang.String | El texto de screenTip para el hipervínculo especificado. |

**Returns:**
int - índice del objeto [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### clear() {#clear--}
```
public void clear()
```


Elimina todos los hipervínculos.

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
public GridHyperlink get(int index)
```


Obtiene el elemento [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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


Obtiene el tamaño del enumerador

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Obtiene el objeto Hyperlink de la celda. Si no hay Hyperlink en la celda, devuelve null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | El objeto GridCell. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Obtiene el objeto Hyperlink de la celda. Si no hay Hyperlink en la celda, devuelve null.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | int | La fila de la celda. |
| columna | int | La columna de la celda. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Elimina el hipervínculo en el área especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área que contiene el hipervínculo. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el hipervínculo en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

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

