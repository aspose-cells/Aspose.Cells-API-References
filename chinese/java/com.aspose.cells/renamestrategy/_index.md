---
title: "RenameStrategy"
second_title: "Aspose.Cells for Java API 参考"
description: "列重复名称的策略选项。"
type: docs
url: /zh/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

列重复名称的策略选项。

**Remarks**

在处理带有标题的数据时，某些场景要求所有列的标题不重复。例如，将数据导出到数据表且标题需作为数据表的列名时，标题的重复值是无效的。对于此类情况，用户可以通过指定此策略来决定如何处理。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DIGIT](#DIGIT) | 名称以数字命名。 |
| [EXCEPTION](#EXCEPTION) | 抛出异常。 |
| [LETTER](#LETTER) | 以字母命名.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


以数字命名。重复的名称将变为 ...1、...2 等。

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


抛出异常。

### LETTER {#LETTER}
```
public static final int LETTER
```


以字母命名.. 重复的名称将变为 ...A、...B 等。

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

