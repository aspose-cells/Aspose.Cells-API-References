---
title: "DataSorterKey"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据排序器的键。"
type: docs
url: /zh/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

表示数据排序器的键。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 获取已排序的颜色。 |
| [getIconId()](#getIconId--) | 表示图标集类型的 id。 |
| [getIconSetType()](#getIconSetType--) | 表示图标集类型。 |
| [getIndex()](#getIndex--) | 获取已排序的列索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [getOrder()](#getOrder--) | 指示排序的顺序。 |
| [getType()](#getType--) | 表示排序的类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


获取已排序的颜色。

**Remarks**

仅在 [getType()](../../com.aspose.cells/datasorterkey\#getType--) 为 [SortOnType.CELL_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) 或 [SortOnType.FONT_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR) 时生效。

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


表示图标集类型的 id。

**Remarks**

仅在 [getType()](../../com.aspose.cells/datasorterkey\#getType--) 为 [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) 时生效。

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


表示图标集类型。

参见[IconSetType](../../com.aspose.cells/iconsettype)。

**Remarks**

仅在 [getType()](../../com.aspose.cells/datasorterkey\#getType--) 为 [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) 时生效。

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取已排序的列索引（绝对位置，列 A 为 0，B 为 1，...）。

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


指示排序的顺序。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


表示排序的类型。

参见 [SortOnType](../../com.aspose.cells/sortontype)。

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

