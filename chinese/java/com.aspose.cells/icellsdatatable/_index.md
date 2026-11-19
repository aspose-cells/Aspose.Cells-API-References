---
title: "ICellsDataTable"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据表。"
type: docs
url: /zh/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

表示数据表。

**Remarks**
## 方法

| 方法 | 描述 |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | 将光标移动到此对象的前面，正好在第一行之前。 |
| [get(int columnIndex)](#get-int-) | 获取由索引指定的列中存储的数据。 |
| [get(String columnName)](#get-java.lang.String-) | 获取由列名指定的列中存储的数据。 |
| [getColumns()](#getColumns--) | 获取列的名称。 |
| [getCount()](#getCount--) | 获取记录的计数。-1 表示记录计数未知。 |
| [next()](#next--) | 将光标从当前位置向下移动一行。 |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


将光标移动到此对象的前面，正好在第一行之前。

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


获取由索引指定的列中存储的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列的零基索引。 |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


获取由列名指定的列中存储的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnName | java.lang.String | 列名。 |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


获取列的名称。

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取记录的计数。-1 表示记录计数未知。

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


将光标从当前位置向下移动一行。

**Returns:**
boolean - 如果新当前行有效；如果没有更多行则为 false
