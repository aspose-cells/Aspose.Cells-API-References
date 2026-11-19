---
title: "ChartSplitType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示饼中饼图或条形饼图的两个部分的分割方式。"
type: docs
url: /zh/java/com.aspose.cells/chartsplittype/
---

**Inheritance:**
java.lang.Object
```
public final class ChartSplitType
```

表示饼中饼图或条形饼图的两个部分的分割方式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [AUTO](#AUTO) | 表示应使用此图表类型的默认机制进行拆分的数据点。 |
| [CUSTOM](#CUSTOM) | 表示应根据自定义拆分值在饼图和第二个图表之间拆分的数据点。 |
| [PERCENT_VALUE](#PERCENT-VALUE) | 表示应通过将百分比低于拆分位置的点放入第二个图表中，在饼图和第二个图表之间拆分的数据点。 |
| [POSITION](#POSITION) | 表示数据点。 |
| [VALUE](#VALUE) | 表示应通过将值低于拆分位置的数据点放入第二个图表中，在饼图和第二个图表之间拆分的数据点。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AUTO {#AUTO}
```
public static final int AUTO
```


表示应使用此图表类型的默认机制进行拆分的数据点。

**Remarks**

注意：此成员现已过时。请改用 Series.IsAutoSplit 属性。自 2023 年 9 月起，此属性将在 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


表示应根据自定义拆分值在饼图和第二个图表之间拆分的数据点。

### PERCENT_VALUE {#PERCENT-VALUE}
```
public static final int PERCENT_VALUE
```


表示应通过将百分比低于拆分位置的点放入第二个图表中，在饼图和第二个图表之间拆分的数据点。

### POSITION {#POSITION}
```
public static final int POSITION
```


表示数据点。数据点应通过将最后的拆分位置放入第二个图表中，在饼图和第二个图表之间拆分。

### VALUE {#VALUE}
```
public static final int VALUE
```


表示应通过将值低于拆分位置的数据点放入第二个图表中，在饼图和第二个图表之间拆分的数据点。

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

