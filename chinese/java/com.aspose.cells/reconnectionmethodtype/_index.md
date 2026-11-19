---
title: "ReConnectionMethodType"
second_title: "Aspose.Cells for Java API 参考"
description: "指定当连接失败时，电子表格应用程序应执行的操作。"
type: docs
url: /zh/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

指定当连接失败时，电子表格应用程序应执行的操作。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALWAYS](#ALWAYS) | 在每次刷新时，从外部连接文件获取更新的连接信息（如果可用），并使用它来替代现有的连接信息。 |
| [NEVER](#NEVER) | 即使外部连接文件可用，且现有的连接信息无效，也永不从外部连接文件获取更新的连接信息。 |
| [REQUIRED](#REQUIRED) | 刷新时使用现有的连接信息，如果它最终无效，则从外部连接文件获取更新的连接信息（如果可用）。 |
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


在每次刷新时，从外部连接文件获取更新的连接信息（如果可用），并使用它来替代现有的连接信息。如果外部连接文件不可用，则数据刷新将失败。

### NEVER {#NEVER}
```
public static final int NEVER
```


即使外部连接文件可用，且现有的连接信息无效，也永不从外部连接文件获取更新的连接信息。

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


刷新时使用现有的连接信息，如果它最终无效，则从外部连接文件获取更新的连接信息（如果可用）。

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

