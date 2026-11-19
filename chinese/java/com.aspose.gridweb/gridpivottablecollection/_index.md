---
title: "GridPivotTableCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

封装一个 [GridPivotTable](../../com.aspose.gridweb/gridpivottable) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | 向 PivotCaches 集合中添加一个新的 PivotTable 缓存。 |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | 向 PivotCaches 集合中添加一个新的 PivotTable 缓存。 |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | 向 PivotCaches 集合中添加一个新的 PivotTable 缓存。 |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | 向 PivotCaches 集合中添加一个新的 PivotTable 缓存。 |
| [clear()](#clear--) | 清除所有 PivotTable。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridPivotTable](../../com.aspose.gridweb/gridpivottable) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的 PivotTable。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


向 PivotCaches 集合中添加一个新的 PivotTable 缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | 源工作表。 |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 源工作表中的区域。 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的缓存索引。
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


向 PivotCaches 集合中添加一个新的 PivotTable 缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| worksheetname | java.lang.String | 源工作表的名称。 |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 源工作表中的区域。 |
| destRow | int | PivotTable 报表目标范围左上角单元格的行号。 |
| destCol | int | PivotTable 报表目标范围左上角单元格的列号。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的缓存索引。
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


向 PivotCaches 集合中添加一个新的 PivotTable 缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| worksheetname | java.lang.String | 源工作表的名称。 |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 源工作表中的区域。 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的缓存索引。
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


向 PivotCaches 集合中添加一个新的 PivotTable 缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | java.lang.String | 新 PivotTable 的数据单元格范围。示例：Sheet1!A1:C8 |
| destCellName | java.lang.String | PivotTable 报表目标范围左上角的单元格。 |
| tableName | java.lang.String | 新 PivotTable 报表的名称。 |

**Returns:**
int - 新添加的缓存索引。
### clear() {#clear--}
```
public void clear()
```


清除所有 PivotTable。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public GridPivotTable get(int index)
```


获取指定索引处的 [GridPivotTable](../../com.aspose.gridweb/gridpivottable) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

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


获取枚举器的大小

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


移除指定索引处的 PivotTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

