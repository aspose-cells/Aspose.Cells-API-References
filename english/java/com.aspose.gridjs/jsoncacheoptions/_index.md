---
title: JsonCacheOptions
second_title: Aspose.Cells for Java API Reference
description: Configuration options for JSON caching in GridJs.
type: docs
url: /java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Configuration options for JSON caching in GridJs. Controls both memory (L1) and disk (L2) cache behavior.
## Constructors

| Constructor | Description |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Gets whether to compress disk cache using Gzip (default: true). |
| [getDiskPath()](#getDiskPath--) | Gets the disk cache directory path. |
| [getEnable()](#getEnable--) | Gets whether to enable JSON caching for faster response. |
| [getEnableDisk()](#getEnableDisk--) | Gets whether to enable disk cache (default: true). |
| [getImplementation()](#getImplementation--) | Gets the custom JSON cache implementation. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Gets the maximum disk cache size in MB (default: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Gets the maximum number of entries in memory cache (default: 1000). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Sets whether to compress disk cache using Gzip (default: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Sets the disk cache directory path. |
| [setEnable(boolean value)](#setEnable-boolean-) | Sets whether to enable JSON caching for faster response. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Sets whether to enable disk cache (default: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Sets the custom JSON cache implementation. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Sets the maximum disk cache size in MB (default: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Sets the maximum number of entries in memory cache (default: 1000). |
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
| Parameter | Type | Description |
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


Gets whether to compress disk cache using Gzip (default: true). Takes effect when Enable = true and using default cache.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Gets the disk cache directory path. Takes effect when Enable = true and using default cache. Default: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Gets whether to enable JSON caching for faster response. When enabled, GridJs will cache the generated JSON and reuse it for subsequent requests. The default value is false. Note: You need to set Implementation to use custom cache storage.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Gets whether to enable disk cache (default: true). Takes effect when Enable = true and using default cache.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Gets the custom JSON cache implementation. If not set, GridJs will use the default memory + disk cache.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Gets the maximum disk cache size in MB (default: 500 MB). Takes effect when Enable = true and using default cache.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Gets the maximum number of entries in memory cache (default: 1000). Takes effect when Enable = true and using default cache.

**Returns:**
int
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


Sets whether to compress disk cache using Gzip (default: true). Takes effect when Enable = true and using default cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Sets the disk cache directory path. Takes effect when Enable = true and using default cache. Default: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Sets whether to enable JSON caching for faster response. When enabled, GridJs will cache the generated JSON and reuse it for subsequent requests. The default value is false. Note: You need to set Implementation to use custom cache storage.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Sets whether to enable disk cache (default: true). Takes effect when Enable = true and using default cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Sets the custom JSON cache implementation. If not set, GridJs will use the default memory + disk cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Sets the maximum disk cache size in MB (default: 500 MB). Takes effect when Enable = true and using default cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Sets the maximum number of entries in memory cache (default: 1000). Takes effect when Enable = true and using default cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

