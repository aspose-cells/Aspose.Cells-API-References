---
title: "ReserveMissingPivotItemType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示如何保留缺失的透视表项。"
type: docs
url: /zh/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

表示如何保留缺失的透视表项。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALL](#ALL) | 保留所有缺失项。 |
| [DEFAULT](#DEFAULT) | 删除旧的缺失透视项，并将新数据源中已删除的项保留为缺失项。 |
| [NONE](#NONE) | 删除所有缺失的透视项。 |
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
### ALL {#ALL}
```
public static final int ALL
```


保留所有缺失项。

**Remarks**

在 Excel 中，只要未关闭 Excel，透视表首次刷新生成的缺失项将被保留，即使多次刷新也如此。

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


删除旧的缺失透视项，并将新数据源中已删除的项保留为缺失项。

### NONE {#NONE}
```
public static final int NONE
```


删除所有缺失的透视项。

**Remarks**

旧缺失的透视项的顺序将被忽略。

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

