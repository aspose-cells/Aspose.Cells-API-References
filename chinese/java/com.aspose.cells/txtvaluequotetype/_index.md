---
title: "TxtValueQuoteType"
second_title: "Aspose.Cells for Java API 参考"
description: "指定文本格式文件中值使用引号的类型。"
type: docs
url: /zh/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

指定文本格式文件中值使用引号的类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALWAYS](#ALWAYS) | 所有值始终会加引号。 |
| [MINIMUM](#MINIMUM) | 仅在需要时为值加引号。 |
| [NEVER](#NEVER) | 所有值将不加引号。 |
| [NORMAL](#NORMAL) | 所有包含特殊字符（如引号、分隔符）的值将加引号。 |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


所有值始终会加引号。

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


仅在需要时为值加引号。例如，如果某个值包含引号但引号不在该值的开头，则该值将不加引号。

### NEVER {#NEVER}
```
public static final int NEVER
```


所有值将不加引号。使用此类型导出的文本文件可能无法正确读取，因为缺少必要的引号。

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


所有包含特殊字符（如引号、分隔符）的值将加引号。这与 Microsoft Excel 导出文本文件的行为相同。

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

