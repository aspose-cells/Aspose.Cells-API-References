---
title: "JsonCacheOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "GridJs 中 JSON 缓存的配置选项。"
type: docs
url: /zh/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

GridJs 中 JSON 缓存的配置选项。控制内存 (L1) 和磁盘 (L2) 缓存的行为。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | 获取是否使用 Gzip 压缩磁盘缓存（默认：true）。 |
| [getDiskPath()](#getDiskPath--) | 获取磁盘缓存目录路径。 |
| [getDiskTtl()](#getDiskTtl--) | 获取磁盘缓存的 TTL（以分钟为单位，默认：1440）。 |
| [getEnable()](#getEnable--) | 获取是否启用 JSON 缓存以获得更快的响应。 |
| [getEnableDisk()](#getEnableDisk--) | 获取是否启用磁盘缓存（默认：true）。 |
| [getImplementation()](#getImplementation--) | 获取自定义 JSON 缓存实现。 |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | 获取磁盘缓存的最大大小（单位 MB，默认：500 MB）。 |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | 获取内存缓存的最大条目数（默认：1000）。 |
| [getMemoryTtl()](#getMemoryTtl--) | 获取内存缓存的 TTL（以分钟为单位，默认：60）。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | 设置是否使用 Gzip 压缩磁盘缓存（默认：true）。 |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | 设置磁盘缓存目录路径。 |
| [setDiskTtl(long value)](#setDiskTtl-long-) | 设置磁盘缓存的 TTL（以分钟为单位，默认：1440）。 |
| [setEnable(boolean value)](#setEnable-boolean-) | 设置是否启用 JSON 缓存以获得更快的响应。 |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | 设置是否启用磁盘缓存（默认：true）。 |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | 设置自定义 JSON 缓存实现。 |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | 设置磁盘缓存的最大大小（单位 MB，默认：500 MB）。 |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | 设置内存缓存的最大条目数（默认：1000）。 |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | 设置内存缓存的 TTL（以分钟为单位，默认：60）。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonCacheOptions() {#JsonCacheOptions--}
```
public JsonCacheOptions()
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


获取是否使用 Gzip 压缩磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


获取磁盘缓存目录路径。当 Enable = true 且使用默认缓存时生效。默认值：[FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


获取磁盘缓存的 TTL（以分钟为单位，默认：1440）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


获取是否启用 JSON 缓存以获得更快的响应。启用后，GridJs 将缓存生成的 JSON 并在后续请求中复用。默认值为 false。注意：需要设置 Implementation 以使用自定义缓存存储。

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


获取是否启用磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


获取自定义 JSON 缓存实现。如果未设置，GridJs 将使用默认的内存 + 磁盘缓存。

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


获取磁盘缓存的最大大小（单位 MB）（默认：500 MB）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


获取内存缓存的最大条目数（默认：1000）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


获取内存缓存的 TTL（分钟）（默认：60）。当 Enable = true 且使用默认缓存时生效。

**Returns:**
long
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




### setCompressDisk(boolean value) {#setCompressDisk-boolean-}
```
public void setCompressDisk(boolean value)
```


设置是否使用 Gzip 压缩磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


设置磁盘缓存目录路径。当 Enable = true 且使用默认缓存时生效。默认值：[FileCacheDirectory]/json\_cache

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


设置磁盘缓存的 TTL（分钟）（默认：1440）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


设置是否启用 JSON 缓存以获得更快的响应。启用后，GridJs 将缓存生成的 JSON 并在后续请求中复用。默认值为 false。注意：需要设置 Implementation 以使用自定义缓存存储。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


设置是否启用磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


设置自定义 JSON 缓存实现。如果未设置，GridJs 将使用默认的内存 + 磁盘缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


设置磁盘缓存的最大大小（单位 MB）（默认：500 MB）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


设置内存缓存的最大条目数（默认：1000）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


设置内存缓存的 TTL（分钟）（默认：60）。当 Enable = true 且使用默认缓存时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | long |  |

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

