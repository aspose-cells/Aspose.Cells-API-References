---
title: "PivotDateTimeRangeGroupSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示按日期时间范围分组的字段。"
type: docs
url: /zh/java/com.aspose.cells/pivotdatetimerangegroupsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
```
public class PivotDateTimeRangeGroupSettings extends PivotFieldGroupSettings
```

表示按日期时间范围分组的字段。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEnd()](#getEnd--) | 获取组的结束日期时间。 |
| [getGroupByTypes()](#getGroupByTypes--) | 获取按日期时间分组的类型。 |
| [getInterval()](#getInterval--) | 获取组的内部。 |
| [getStart()](#getStart--) | 获取组的开始日期时间。 |
| [getType()](#getType--) | 获取数据时间组类型。 |
| [hashCode()](#hashCode--) |  |
| [isGroupedBy(int type)](#isGroupedBy-int-) | 检查字段是否按该类型分组。 |
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
### getEnd() {#getEnd--}
```
public DateTime getEnd()
```


获取组的结束日期时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getGroupByTypes() {#getGroupByTypes--}
```
public int[] getGroupByTypes()
```


获取按日期时间分组的类型。

参见 [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


获取组的内部。

**Returns:**
double
### getStart() {#getStart--}
```
public DateTime getStart()
```


获取组的开始日期时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getType() {#getType--}
```
public int getType()
```


获取数据时间组类型。

参见 [PivotFieldGroupType](../../com.aspose.cells/pivotfieldgrouptype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGroupedBy(int type) {#isGroupedBy-int-}
```
public boolean isGroupedBy(int type)
```


检查字段是否按该类型分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。组类型 |

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

