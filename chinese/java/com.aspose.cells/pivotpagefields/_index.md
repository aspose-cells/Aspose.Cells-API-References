---
title: "PivotPageFields"
second_title: "Aspose.Cells for Java API 参考"
description: "表示透视表数据源为合并范围时的透视页项目。"
type: docs
url: /zh/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

表示透视表数据源为合并范围时的透视页项目。它最多只能包含 4 项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | 表示透视页字段项目。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | 设置每个页面字段中用于标识数据范围的项标签。 |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | 添加一个页面字段。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | 获取页面字段的数量。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


表示透视页字段项目。

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


设置每个页面字段中用于标识数据范围的项标签。pageItemIndex.Length 必须等于 PageFieldCount，因此请先添加页面字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rangeIndex | int | 合并数据范围索引。 |
| pageItemIndex | int[] | 每个页面字段中的页面项索引。pageItemIndex[2] = 1 表示在第三个字段中的第二个项用于标识此范围。pageItemIndex[1] = -1 表示在第二个字段中没有项用于标识此范围，MS 将自动创建 \"blank\" 项在第二个字段中以标识此范围。 |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


添加一个页面字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageItems | java.lang.String[] | 页面字段项标签 |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


获取页面字段的数量。

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

