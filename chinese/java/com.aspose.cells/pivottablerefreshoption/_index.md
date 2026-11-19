---
title: "PivotTableRefreshOption"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 pivot table 刷新数据源的选项。"
type: docs
url: /zh/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

表示 pivot table 刷新数据源的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | 表示 pivot table 刷新数据源的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | 指示在最大值和最小值保持不变时是否保留缓存的本地组数据。 |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | 表示如何保留缺失的透视项。 |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | 指示是否保持透视项的原始顺序与旧数据源相同。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | 指示在最大值和最小值保持不变时是否保留缓存的本地组数据。 |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | 指示是否保持透视项的原始顺序与旧数据源相同。 |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | 表示如何保留缺失的透视项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


表示 pivot table 刷新数据源的选项。

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


指示在最大值和最小值保持不变时是否保留缓存的本地组数据。默认值为 false，表示使用本地设置刷新组。

**Remarks**

这是一种临时解决方案，请通过实现 [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) 来本地化透视表。

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


表示如何保留缺失的透视项。

参见 [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


指示是否保持透视项的原始顺序与旧数据源相同。

**Remarks**

仅适用于未排序的透视字段。刷新此类透视字段时，Ms Excel 会保持旧数据源的原始顺序。此属性的默认值为 true，表示与 Ms Excel 相同的行为。如果用户需要透视字段完全按照新数据源中的数据进行刷新，则应将此属性设置为 false。

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




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


指示在最大值和最小值保持不变时是否保留缓存的本地组数据。默认值为 false，表示使用本地设置刷新组。

**Remarks**

这是一种临时解决方案，请通过实现 [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) 来本地化透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


指示是否保持透视项的原始顺序与旧数据源相同。

**Remarks**

仅适用于未排序的透视字段。刷新此类透视字段时，Ms Excel 会保持旧数据源的原始顺序。此属性的默认值为 true，表示与 Ms Excel 相同的行为。如果用户需要透视字段完全按照新数据源中的数据进行刷新，则应将此属性设置为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


表示如何保留缺失的透视项。

参见 [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype)。

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

