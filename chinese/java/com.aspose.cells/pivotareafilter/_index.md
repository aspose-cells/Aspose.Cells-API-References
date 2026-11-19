---
title: "PivotAreaFilter"
second_title: "Aspose.Cells for Java API 参考"
description: "表示  的过滤器，用于 。"
type: docs
url: /zh/java/com.aspose.cells/pivotareafilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotAreaFilter
```

表示 [PivotArea](../../com.aspose.cells/pivotarea) 对于 [PivotTable](../../com.aspose.cells/pivottable) 的过滤器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotAreaFilter()](#PivotAreaFilter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | 获取此过滤器所引用的源字段中的字段索引。 |
| [getSelected()](#getSelected--) | 指示此字段是否具有选择。 |
| [hashCode()](#hashCode--) |  |
| [isSubtotalSet(int subtotalType)](#isSubtotalSet-int-) | 获取为此过滤器设置的汇总方式。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setSelected(boolean value)](#setSelected-boolean-) | 指示此字段是否具有选择。 |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | 过滤器的汇总。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotAreaFilter() {#PivotAreaFilter--}
```
public PivotAreaFilter()
```


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
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


获取此过滤器所引用的源字段中的字段索引。值为 -2 表示值字段。

**Returns:**
int
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


指示此字段是否具有选择。仅在 PivotTable 处于大纲视图时有效。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSubtotalSet(int subtotalType) {#isSubtotalSet-int-}
```
public boolean isSubtotalSet(int subtotalType)
```


获取为此过滤器设置的汇总方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。汇总函数类型。 |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


指示此字段是否具有选择。仅在 PivotTable 处于大纲视图时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


过滤器的汇总。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。汇总函数。 |
| 显示 | boolean | 指示是否显示此汇总数据。 |

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

