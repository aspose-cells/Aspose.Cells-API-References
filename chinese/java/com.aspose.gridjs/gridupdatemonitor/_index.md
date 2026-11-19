---
title: "GridUpdateMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "用于用户跟踪更新操作变化的监视器。"
type: docs
url: /zh/java/com.aspose.gridjs/gridupdatemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridUpdateMonitor
```

用于用户跟踪更新操作变化的监视器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridUpdateMonitor()](#GridUpdateMonitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [afterUpdate(String op, String uid, ArrayList cells)](#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-) | 更新操作后 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridUpdateMonitor() {#GridUpdateMonitor--}
```
public GridUpdateMonitor()
```


### afterUpdate(String op, String uid, ArrayList cells) {#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-}
```
public abstract void afterUpdate(String op, String uid, ArrayList cells)
```


更新操作后

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| op | java.lang.String | 更新操作的 JSON 字符串 |
| uid | java.lang.String | 文件缓存的唯一 ID。 |
| 单元格 | java.util.ArrayList | 已更新单元格列表，包括样式更改、数值更改或公式更改的单元格 |

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

