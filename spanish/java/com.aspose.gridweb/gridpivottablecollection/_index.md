---
title: "GridPivotTableCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Encapsula una colección de objetos [GridPivotTable](../../com.aspose.gridweb/gridpivottable).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Agrega una nueva caché de PivotTable a una colección PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Agrega una nueva caché de PivotTable a una colección PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Agrega una nueva caché de PivotTable a una colección PivotCaches. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Agrega una nueva caché de PivotTable a una colección PivotCaches. |
| [clear()](#clear--) | Limpia todas las PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [GridPivotTable](../../com.aspose.gridweb/gridpivottable) en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el tamaño del enumerador |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina la PivotTable en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Agrega una nueva caché de PivotTable a una colección PivotCaches.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | La hoja de cálculo fuente. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área en la hoja de cálculo fuente. |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice de caché añadido.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Agrega una nueva caché de PivotTable a una colección PivotCaches.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheetname | java.lang.String | El nombre de la hoja de cálculo fuente. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área en la hoja de cálculo fuente. |
| destRow | int | La fila de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| destCol | int | La columna de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice de caché añadido.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Agrega una nueva caché de PivotTable a una colección PivotCaches.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheetname | java.lang.String | El nombre de la hoja de cálculo fuente. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | El área en la hoja de cálculo fuente. |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice de caché añadido.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Agrega una nueva caché de PivotTable a una colección PivotCaches.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | java.lang.String | El rango de celdas de datos para el nuevo PivotTable. Ejemplo: Sheet1!A1:C8 |
| destCellName | java.lang.String | La celda en la esquina superior izquierda del rango de destino del informe de PivotTable. |
| tableName | java.lang.String | El nombre del nuevo informe de PivotTable. |

**Returns:**
int - El índice de caché añadido.
### clear() {#clear--}
```
public void clear()
```


Limpia todas las PivotTables.

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
public GridPivotTable get(int index)
```


Obtiene el elemento [GridPivotTable](../../com.aspose.gridweb/gridpivottable) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina la PivotTable en el índice especificado.

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

