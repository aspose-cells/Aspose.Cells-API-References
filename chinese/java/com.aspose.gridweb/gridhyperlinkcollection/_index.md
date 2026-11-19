---
title: "GridHyperlinkCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

封装一个 [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | 向指定单元格添加超链接。 |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [clear()](#clear--) | 清除所有超链接。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | 获取单元格的 Hyperlink 对象。 |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | 获取单元格的 Hyperlink 对象。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | 移除指定区域的超链接。 |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的超链接。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


向指定的单元格或单元格范围添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 超链接范围的第一行。 |
| firstColumn | int | 超链接范围的第一列。 |
| totalRows | int | 此超链接范围的行数。 |
| totalColumns | int | 此超链接范围的列数。 |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 对象索引。
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


向指定的单元格或单元格范围添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |
| totalRows | int | 此超链接范围的行数。 |
| totalColumns | int | 此超链接范围的列数。 |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 对象索引。
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


向指定单元格添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 对象索引。
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


向指定的单元格或单元格范围添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startCellName | java.lang.String | 范围的左上单元格。 |
| endCellName | java.lang.String | 范围的右下单元格。 |
| 地址 | java.lang.String | 超链接的地址。 |
| textToDisplay | java.lang.String | 指定超链接要显示的文本。 |
| screenTip | java.lang.String | 指定超链接的屏幕提示文本。 |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 对象索引。
### clear() {#clear--}
```
public void clear()
```


清除所有超链接。

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
public GridHyperlink get(int index)
```


获取指定索引处的 [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

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


获取枚举器的大小

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


获取单元格的 Hyperlink 对象。如果单元格没有 Hyperlink，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | GridCell 对象。 |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


获取单元格的 Hyperlink 对象。如果单元格没有 Hyperlink，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格的行号。 |
| 列 | int | 单元格的列号。 |

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


移除指定区域的超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 包含超链接的区域。 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的超链接。

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

