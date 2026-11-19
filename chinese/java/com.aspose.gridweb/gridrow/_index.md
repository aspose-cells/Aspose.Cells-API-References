---
title: "GridRow"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示电子表格中单个图片的对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

封装表示电子表格中单个图片的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | 获取单元格。 |
| [getCellByIndex(int index)](#getCellByIndex-int-) | 通过列表中的特定索引获取单元格。 |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | 获取行中的第一个单元格。 |
| [getHeight()](#getHeight--) | 获取以点为单位的行高。 |
| [getHidden()](#getHidden--) | 指示该行是否隐藏。 |
| [getIndex()](#getIndex--) | 获取此行的索引。 |
| [getLastCell()](#getLastCell--) | 获取行中的最后一个单元格。 |
| [getLastDataCell()](#getLastDataCell--) | 获取行中的最后一个单元格。 |
| [getOutlineLevel()](#getOutlineLevel--) | 获取大纲级别。 |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | 指示该行是否包含任何数据 |
| [iterator()](#iterator--) | 获取单元格枚举器 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | 设置以点为单位的行高。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示该行是否隐藏。 |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | 设置大纲级别。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


获取单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


通过列表中的特定索引获取单元格。

**Remarks**

注意：此成员已过时。请改用 Row.GetEnumerator() 方法遍历此行中的所有单元格。此属性将在自 2015 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 位置。 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


获取行中的第一个单元格。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取以点为单位的行高。

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


指示该行是否隐藏。

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取此行的索引。

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


获取行中的最后一个单元格。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


获取行中的最后一个单元格。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


获取大纲级别。

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


指示该行是否包含任何数据

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取单元格枚举器

**Returns:**
java.util.Iterator - cells 枚举器
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


设置以点为单位的行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


指示该行是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


设置大纲级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte |  |

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

