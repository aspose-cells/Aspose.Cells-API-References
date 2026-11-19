---
title: "PivotTableCalculateOption"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 pivot table 计算数据的选项。"
type: docs
url: /zh/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

表示 pivot table 计算数据的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | 指示刷新图表是否基于此数据透视表。 |
| [getRefreshData()](#getRefreshData--) | 指示是否刷新数据透视表的数据源。 |
| [getRefreshOption()](#getRefreshOption--) | 获取用于将数据源刷新到数据透视缓存的选项。 |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | 表示如何保留缺失的透视项。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | 指示刷新图表是否基于此数据透视表。 |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | 指示是否刷新数据透视表的数据源。 |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | 设置用于将数据源刷新到数据透视缓存的选项。 |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | 表示如何保留缺失的透视项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
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
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


指示刷新图表是否基于此数据透视表。

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


指示是否刷新数据透视表的数据源。

**Remarks**

如果为 true，则从数据源刷新数据透视缓存，然后基于相同的数据透视缓存计算所有数据透视表。

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


获取用于将数据源刷新到数据透视缓存的选项。

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


表示如何保留缺失的透视项。

参见 [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype)。

**Remarks**

仅在 [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) 为 true 时有效。

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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


指示刷新图表是否基于此数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


指示是否刷新数据透视表的数据源。

**Remarks**

如果为 true，则从数据源刷新数据透视缓存，然后基于相同的数据透视缓存计算所有数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


设置用于将数据源刷新到数据透视缓存的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


表示如何保留缺失的透视项。

参见 [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype)。

**Remarks**

仅在 [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) 为 true 时有效。

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

