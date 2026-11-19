---
title: "SessionMode"
second_title: "Aspose.Cells for Java API 参考"
description: "表示网格的会话模式。"
type: docs
url: /zh/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

表示网格的会话模式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [CUSTOM](#CUSTOM) | 使用 LoadCustomData 事件手动加载网格的工作表数据。 |
| [FILE](#FILE) | 使用系统文件自动存储/恢复网格的工作表数据，用户需要设置 SessionStorePath 来指定文件目录。 |
| [SESSION](#SESSION) | 使用系统会话自动存储/恢复网格的工作表数据。 |
| [VIEW_STATE](#VIEW-STATE) | 使用页面的 viewstate 自动存储/恢复网格的工作表数据。 |
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
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


使用 LoadCustomData 事件手动加载网格的工作表数据，并使用 SheetDataUpdated 事件保存网格的工作表数据。

### FILE {#FILE}
```
public static final int FILE
```


使用系统文件自动存储/恢复网格的工作表数据，用户需要设置 SessionStorePath 来指定文件目录。

### SESSION {#SESSION}
```
public static final int SESSION
```


使用系统会话自动存储/恢复网格的工作表数据。

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


使用页面的 viewstate 自动存储/恢复网格的工作表数据。

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

