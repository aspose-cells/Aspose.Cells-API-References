---
title: "GridCacheForStream"
second_title: "Aspose.Cells for Java API 参考"
description: "此类包含 GridJs 的缓存操作。"
type: docs
url: /zh/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

此类包含针对 GridJs 的缓存操作。用户应基于它实现自己的存储业务逻辑。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | 实现此方法以从缓存获取文件 URL。 |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | 检查具有 uid 的缓存是否存在 |
| [loadStream(String uid)](#loadStream-java.lang.String-) | 实现此方法以使用键 uid 加载缓存，并返回缓存中的流。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | 实现此方法以保存缓存，将流使用键 uid 保存到缓存中。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
```


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
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


实现此方法以从缓存获取文件 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
java.lang.String - 文件的 URL
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


检查具有 uid 的缓存是否存在

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件缓存的唯一 ID。 |

**Returns:**
boolean - 布尔值
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


实现此方法以使用键 uid 加载缓存，并返回缓存中的流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


实现此方法以保存缓存，将流使用键 uid 保存到缓存中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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

