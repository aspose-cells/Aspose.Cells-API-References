---
title: "GridWorksheetCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

封装一个 [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 向集合中添加工作表。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String sheetName)](#add-java.lang.String-) | 向集合中添加工作表。 |
| [addCopy(int sheetIndex)](#addCopy-int-) | 向集合中添加工作表并从已有工作表复制数据。 |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | 向集合中添加工作表并从已有工作表复制数据。 |
| [calculateFormula()](#calculateFormula--) | 计算公式的结果。 |
| [clear()](#clear--) | 清除所有工作表。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 元素。 |
| [get(String sheetName)](#get-java.lang.String-) | 获取具有指定名称的 [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 元素。 |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | 表示打开电子表格时活动工作表的索引。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取枚举器的大小 |
| [getDefaultFontName()](#getDefaultFontName--) | 获取控件的默认字体名称。 |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | 获取电子表格中所有 Name 对象的集合。 |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | 获取用于格式化/解析数值的十进制分隔符。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | 插入工作表。 |
| [iterator()](#iterator--) | 获取行枚举器 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 删除指定索引处的元素。 |
| [removeAt(String name)](#removeAt-java.lang.String-) | 删除指定名称的元素。 |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | 表示打开电子表格时活动工作表的索引。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 设置控件的默认字体名称。 |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | 设置数值格式化/解析的十进制分隔符。 |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | 设置工作表的可见性。 |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | 交换这两个工作表. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


向集合中添加工作表。

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 对象索引。
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


向集合中添加工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表名称 |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


向集合中添加工作表并从已有工作表复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 源工作表的索引. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 对象索引。
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


向集合中添加工作表并从已有工作表复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 源工作表的名称. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 对象索引。
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


计算公式的结果。

### clear() {#clear--}
```
public void clear()
```


清除所有工作表。

**Remarks**

工作簿必须包含一个工作表.

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
public GridWorksheet get(int index)
```


获取指定索引处的 [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


获取具有指定名称的 [GridWorksheet](../../com.aspose.gridweb/gridworksheet) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表的名称。 |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


表示打开电子表格时活动工作表的索引。

**Remarks**

工作表索引从零开始.

**Returns:**
int
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


获取控件的默认字体名称。

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


获取电子表格中所有 Name 对象的集合。

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


获取数值格式化/解析时的十进制分隔符。默认是当前地区的十进制分隔符。

**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


插入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 工作表索引 |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取行枚举器

**Returns:**
java.util.Iterator - 行枚举器
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


删除指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的元素的索引值。 |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


删除指定名称的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 要删除的元素的名称。 |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


表示打开电子表格时活动工作表的索引。

**Remarks**

工作表索引从零开始.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


设置控件的默认字体名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


设置数值格式化/解析的十进制分隔符。默认值为当前地区的十进制分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


设置工作表的可见性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 源工作表的名称. |
| isVisible | boolean | 工作表是否可见 |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


交换这两个工作表.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex1 | int | 第一个工作表。 |
| sheetIndex2 | int | 第二个工作表。 |

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

