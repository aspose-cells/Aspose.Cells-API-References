---
title: "ICellsDataTable"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una tabla de datos."
type: docs
url: /es/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Representa una tabla de datos.

**Remarks**
## Métodos

| Método | Descripción |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Mueva el cursor al inicio de este objeto, justo antes de la primera fila. |
| [get(int columnIndex)](#get-int-) | Obtiene los datos almacenados en la columna especificada por índice. |
| [get(String columnName)](#get-java.lang.String-) | Obtiene los datos almacenados en la columna especificada por nombre de columna. |
| [getColumns()](#getColumns--) | Obtiene el nombre de las columnas. |
| [getCount()](#getCount--) | Obtiene el recuento de los registros. -1 para recuento de registros desconocido. |
| [next()](#next--) | Mueve el cursor una fila hacia abajo desde su posición actual. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Mueva el cursor al inicio de este objeto, justo antes de la primera fila.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Obtiene los datos almacenados en la columna especificada por índice.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | El índice basado en cero de la columna. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Obtiene los datos almacenados en la columna especificada por nombre de columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnName | java.lang.String | El nombre de la columna. |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Obtiene el nombre de las columnas.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el recuento de los registros. -1 para recuento de registros desconocido.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Mueve el cursor una fila hacia abajo desde su posición actual.

**Returns:**
boolean - si la nueva fila actual es válida; false si no hay más filas
