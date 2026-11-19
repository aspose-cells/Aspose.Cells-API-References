---
title: "MergedCellsShrinkType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在删除空行/列等操作时收缩合并单元格的策略。"
type: docs
url: /zh/java/com.aspose.cells/mergedcellsshrinktype/
---

**Inheritance:**
java.lang.Object
```
public final class MergedCellsShrinkType
```

表示在删除空行/列等操作时收缩合并单元格的策略。
## 字段

| 字段 | 描述 |
| --- | --- |
| [KEEP_HEADER_ONLY](#KEEP-HEADER-ONLY) | 仅在合并区域的左上单元格不为空时，保留合并区域的标题行/列。 |
| [NONE](#NONE) | 保持合并单元格不变，不进行任何修改。 |
| [SHRINK_TO_FIT](#SHRINK-TO-FIT) | 在需要时收缩合并区域，通过删除底部的行或右侧的列，同时确保所有内容保持可见。 |
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
### KEEP_HEADER_ONLY {#KEEP-HEADER-ONLY}
```
public static final int KEEP_HEADER_ONLY
```


仅在合并区域的左上单元格不为空时，保留合并区域的标题行/列。

### NONE {#NONE}
```
public static final int NONE
```


保持合并单元格不变，不进行任何修改。

### SHRINK_TO_FIT {#SHRINK-TO-FIT}
```
public static final int SHRINK_TO_FIT
```


在需要时收缩合并区域，通过删除底部的行或右侧的列，同时确保所有内容保持可见。

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

