---
title: "DataSorter"
second_title: "Aspose.Cells for Java API 参考"
description: "DataSorter 的摘要描述。"
type: docs
url: /zh/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

DataSorter 的摘要描述。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | 添加颜色排序键。 |
| [addKey(int key, int order)](#addKey-int-int-) | 添加已排序列索引和排序顺序。 |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | 添加已排序列索引和排序顺序（使用自定义排序列表）。 |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | 添加已排序列索引和排序顺序（使用自定义排序列表）。 |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | 添加已排序列索引和排序顺序（使用自定义排序列表）。 |
| [clear()](#clear--) | 清除所有设置。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | 获取比较字符串时是否区分大小写。 |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | 表示第一排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [getKey2()](#getKey2--) | 表示第二排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [getKey3()](#getKey3--) | 表示第三排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [getKeys()](#getKeys--) | 获取数据排序器的键列表。 |
| [getOrder1()](#getOrder1--) | 表示第一个键的排序顺序。 |
| [getOrder2()](#getOrder2--) | 表示第二个键的排序顺序。 |
| [getOrder3()](#getOrder3--) | 表示第三个键的排序顺序。 |
| [getSortAsNumber()](#getSortAsNumber--) | 指示是否对看起来像数字的内容进行排序。 |
| [getSortLeftToRight()](#getSortLeftToRight--) | True 表示排序方向从左到右。 |
| [hasHeaders()](#hasHeaders--) | 表示该范围是否有标题行。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | 设置比较字符串时是否区分大小写。 |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | 表示该范围是否有标题行。 |
| [setKey1(int value)](#setKey1-int-) | 表示第一排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [setKey2(int value)](#setKey2-int-) | 表示第二排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [setKey3(int value)](#setKey3-int-) | 表示第三排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [setOrder1(int value)](#setOrder1-int-) | 表示第一个键的排序顺序。 |
| [setOrder2(int value)](#setOrder2-int-) | 表示第二个键的排序顺序。 |
| [setOrder3(int value)](#setOrder3-int-) | 表示第三个键的排序顺序。 |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | 指示是否对看起来像数字的内容进行排序。 |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | True 表示排序方向从左到右。 |
| [sort()](#sort--) | 对范围内的数据进行排序。 |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | 对区域的数据进行排序。 |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | 对区域的数据进行排序。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


添加颜色排序键。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | int | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). 已排序颜色值类型。 |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). 排序顺序。 |
| color | [Color](../../com.aspose.cells/color) | 自定义排序颜色。 |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


添加已排序列索引和排序顺序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | int | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). 排序顺序 |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


添加已排序列索引和排序顺序（使用自定义排序列表）。

**Remarks**

如果类型是 SortOnType.CellColor 或 SortOnType.FontColor，customList 为 Color。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | int | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). 排序的值类型。 |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). 排序顺序。 |
| customList | java.lang.Object | 自定义排序列表。 |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


添加已排序列索引和排序顺序（使用自定义排序列表）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | int | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). 排序顺序。 |
| customList | java.lang.String | 自定义排序列表。 |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


添加已排序列索引和排序顺序（使用自定义排序列表）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | int | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). 排序顺序。 |
| customList | java.lang.String[] | 自定义排序列表。 |

### clear() {#clear--}
```
public void clear()
```


清除所有设置。

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


获取比较字符串时是否区分大小写。

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


表示第一排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


表示第二排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


表示第三排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


获取数据排序器的键列表。

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


表示第一个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


表示第二个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


表示第三个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


指示是否对看起来像数字的内容进行排序。

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True 表示排序方向从左到右。False 表示排序方向从上到下。默认值为 false。

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


表示该范围是否有标题行。

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


设置比较字符串时是否区分大小写。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


表示该范围是否有标题行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


表示第一排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


表示第二排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


表示第三排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


表示第一个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


表示第二个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


表示第三个键的排序顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


指示是否对看起来像数字的内容进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True 表示排序方向从左到右。False 表示排序方向从上到下。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


对范围内的数据进行排序。

**Returns:**
int[] - 已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。如果此排序操作不需要移动任何行/列，将返回 null。
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


对区域的数据进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | 单元格包含数据区域。 |
| area | [CellArea](../../com.aspose.cells/cellarea) | 需要排序的区域 |

**Returns:**
int[] - 已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。如果此排序操作不需要移动任何行/列，将返回 null。
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


对区域的数据进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | 单元格包含数据区域。 |
| startRow | int | 区域的起始行。 |
| startColumn | int | 区域的起始列。 |
| endRow | int | 区域的结束行。 |
| endColumn | int | 区域的结束列。 |

**Returns:**
int[] - 已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。如果此排序操作不需要移动任何行/列，将返回 null。
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

