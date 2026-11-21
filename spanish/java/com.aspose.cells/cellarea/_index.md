---
title: "CellArea"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un área de celdas."
type: docs
url: /es/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Representa un área de celdas.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
| [EndColumn](#EndColumn) | Obtiene o establece la columna final de esta área. |
| [EndRow](#EndRow) | Obtiene o establece la fila final de esta área. |
| [StartColumn](#StartColumn) | Obtiene o establece la columna inicial de esta área. |
| [StartRow](#StartRow) | Obtiene o establece la fila inicial de esta área. |
## Métodos

| Método | Descripción |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Compara dos objetos CellArea según su esquina superior izquierda. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Crea un área de celdas. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Crea un área de celdas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto actual de área de celdas. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Obtiene o establece la columna final de esta área.

### EndRow {#EndRow}
```
public int EndRow
```


Obtiene o establece la fila final de esta área.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Obtiene o establece la columna inicial de esta área.

### StartRow {#StartRow}
```
public int StartRow
```


Obtiene o establece la fila inicial de esta área.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Compara dos objetos CellArea según su esquina superior izquierda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - Si dos esquinas están en filas diferentes, entonces compare sus índices de fila. De lo contrario compare sus índices de columna. Si las dos esquinas son iguales, se devolverá 0.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Crea un área de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial. |
| endRow | int | La fila final. |
| endColumn | int | La columna final. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Crea un área de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCellName | java.lang.String | La celda superior izquierda del rango. |
| endCellName | java.lang.String | La celda inferior derecha del rango. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto actual de área de celdas.

**Returns:**
java.lang.String -
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

