---
title: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Java API 参考"
description: "指定在将字符串值转换为数字或日期时间时如何为解析后的值应用样式。"
type: docs
url: /zh/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

指定在将字符串值转换为数字或日期时间时如何为解析后的值应用样式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | 当解析值为普通数字/日期时间值时，将样式设置为内置的数字/日期时间样式。 |
| [EXACT_FORMAT](#EXACT-FORMAT) | 为解析值设置精确的自定义格式，使格式化后的值与原始输入保持一致。 |
| [NONE](#NONE) | 不为解析值设置样式。 |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


当解析值为普通数字/日期时间值时，将样式设置为内置的数字/日期时间样式。

**Remarks**

当 Microsoft Excel 根据用户输入（例如 CSV 文件）解析日期时间或数值时，这些值的格式可能会被更改，例如数字的前导/尾随零、日期时间的年/月/日顺序等。此类型用于模拟 Microsoft Excel 的行为。

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


为解析值设置精确的自定义格式，使格式化后的值与原始输入保持一致。

### NONE {#NONE}
```
public static final int NONE
```


不为解析值设置样式。

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

