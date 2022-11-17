---
title: ICellsDataTable
second_title: Aspose.Cells for Java API Reference
description: Represents data table.
type: docs
weight: 673
url: /java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Represents data table.
## Methods

| Method | Description |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Move the cursor to the front of this object, just before the first row. |
| [get(int columnIndex)](#get-int-) | Gets the data stored in the column specified by index. |
| [get(String columnName)](#get-java.lang.String-) | Gets the data stored in the column specified by column name. |
| [next()](#next--) | Moves the cursor down one row from its current position. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Move the cursor to the front of this object, just before the first row.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Gets the data stored in the column specified by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int | The zero-based index of the column. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Gets the data stored in the column specified by column name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | The column name. |

**Returns:**
java.lang.Object - 
### next() {#next--}
```
public abstract boolean next()
```


Moves the cursor down one row from its current position.

**Returns:**
boolean - if the new current row is valid; false if there are no more rows