---
title: "HyperlinkCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/hyperlinkcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```

封装一个包含 [Hyperlink](../../com.aspose.cells/hyperlink) 对象的集合。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Get Hyperlinks Collection
         HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
 
         //Adding a hyperlink to a URL at "A1" cell
         hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [clear()](#clear--) | 清除所有超链接。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Hyperlink](../../com.aspose.cells/hyperlink) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除此集合中指定索引处的超链接。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


向指定的单元格或单元格范围添加超链接。

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook();
         Worksheet worksheet = excel.getWorksheets().get(0);
         worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
         worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 超链接范围的第一行。 |
| firstColumn | int | 超链接范围的第一列。 |
| totalRows | int | 此超链接范围的行数。 |
| totalColumns | int | 此超链接范围的列数。 |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
int - [Hyperlink](../../com.aspose.cells/hyperlink) 对象索引。
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
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
int - [Hyperlink](../../com.aspose.cells/hyperlink) 对象索引。
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
int - [Hyperlink](../../com.aspose.cells/hyperlink) 对象索引。
### clear() {#clear--}
```
public void clear()
```


清除所有超链接。

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
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
public Hyperlink get(int index)
```


获取指定索引处的 [Hyperlink](../../com.aspose.cells/hyperlink) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
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


移除此集合中指定索引处的超链接。

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

