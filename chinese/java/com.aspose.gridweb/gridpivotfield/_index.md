---
title: "GridPivotField"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视表报告中的字段。"
type: docs
url: /zh/java/com.aspose.gridweb/gridpivotfield/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotField
```

表示数据透视表报告中的字段。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDisplayName()](#getDisplayName--) | 表示 PivotField 的显示名称。 |
| [getFunction()](#getFunction--) | 表示用于汇总 PivotTable 数据字段的函数。 |
| [getPosition()](#getPosition--) | 表示 PivotFields 中的 PivotField 索引。 |
| [hashCode()](#hashCode--) |  |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | 设置数据字段中特定 PivotItem 是否隐藏。 |
| [hideItemByName(String name, boolean isHidden)](#hideItemByName-java.lang.String-boolean-) | 设置数据字段中特定 PivotItem 是否隐藏。 |
| [hideItemByValue(String value, boolean isHidden)](#hideItemByValue-java.lang.String-boolean-) | 设置数据字段中特定 PivotItem 是否隐藏。 |
| [isAscendSort()](#isAscendSort--) | 指示指定的 PivotTable 字段是否已自动升序排序。 |
| [isAutoSort()](#isAutoSort--) | 指示指定的 PivotTable 字段是否已自动排序。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | 指示指定的 PivotTable 字段是否已自动升序排序。 |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | 指示指定的 PivotTable 字段是否已自动排序。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 表示 PivotField 的显示名称。 |
| [setFunction(int value)](#setFunction-int-) | 表示用于汇总 PivotTable 数据字段的函数。 |
| [setPosition(int value)](#setPosition-int-) | 表示 PivotFields 中的 PivotField 索引。 |
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
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


表示 PivotField 的显示名称。

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


表示用于汇总 PivotTable 数据字段的函数。

参见 [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction)。

**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```


表示 PivotFields 中的 PivotField 索引。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


设置数据字段中特定 PivotItem 是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | pivotField 中 pivotItem 的索引。 |
| isHidden | boolean | 特定 PivotItem 是否隐藏 |

### hideItemByName(String name, boolean isHidden) {#hideItemByName-java.lang.String-boolean-}
```
public void hideItemByName(String name, boolean isHidden)
```


设置数据字段中特定 PivotItem 是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | pivotField 中 pivotItem 的名称。 |
| isHidden | boolean | 特定 PivotItem 是否隐藏 |

### hideItemByValue(String value, boolean isHidden) {#hideItemByValue-java.lang.String-boolean-}
```
public void hideItemByValue(String value, boolean isHidden)
```


设置数据字段中特定 PivotItem 是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | pivotField 中 pivotItem 的值。 |
| isHidden | boolean | 特定 PivotItem 是否隐藏 |

### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


指示指定的 PivotTable 字段是否已自动升序排序。

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


指示指定的 PivotTable 字段是否已自动排序。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


指示指定的 PivotTable 字段是否已自动升序排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


指示指定的 PivotTable 字段是否已自动排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


表示 PivotField 的显示名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


表示用于汇总 PivotTable 数据字段的函数。

参见 [GridPivotFieldFunction](../../com.aspose.gridweb/gridpivotfieldfunction)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


表示 PivotFields 中的 PivotField 索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

