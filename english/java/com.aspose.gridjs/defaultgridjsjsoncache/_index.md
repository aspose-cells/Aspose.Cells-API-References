---
title: DefaultGridJsJsonCache
second_title: Aspose.Cells for Java API Reference
description: u699bu6a3fue17bu9428
type: docs
url: /java/com.aspose.gridjs/defaultgridjsjsoncache/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
```
public class DefaultGridJsJsonCache implements IGridJsJsonCache
```

\\u699b\\u6a3f\\ue17b\\u9428?JSON \\u7f02\\u64b3\\u74e8\\u7039\\u70b5\\u5e47\\u951b\\u57201 \\u9350\\u546d\\u74e8 + L2 \\u7ebe\\u4f7a\\u6d0f\\u951b?
## Constructors

| Constructor | Description |
| --- | --- |
| [DefaultGridJsJsonCache(GridJsOptions options)](#DefaultGridJsJsonCache-com.aspose.gridjs.GridJsOptions-) | \\u6d63\\u8de8\\u6564 GridJsOptions \\u95b0\\u5d87\\u7586\\u9352\\u6d98\\u7f13\\u7f02\\u64b3\\u74e8\\u7039\\u70b0\\u7de5 |
| [DefaultGridJsJsonCache()](#DefaultGridJsJsonCache--) | \\u6d63\\u8de8\\u6564\\u934f\\u3125\\u772c Config \\u95b0\\u5d87\\u7586\\u9352\\u6d98\\u7f13\\u7f02\\u64b3\\u74e8\\u7039\\u70b0\\u7de5\\u951b\\u581f\\u68e4\\u9359\\u509b\\u702f\\u95ab\\u72b2\\u56b1\\u93c1\\u5e2e\\u7d1a |
## Methods

| Method | Description |
| --- | --- |
| [clearAll()](#clearAll--) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) |  |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) |  |
| [toString()](#toString--) |  |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DefaultGridJsJsonCache(GridJsOptions options) {#DefaultGridJsJsonCache-com.aspose.gridjs.GridJsOptions-}
```
public DefaultGridJsJsonCache(GridJsOptions options)
```


\\u6d63\\u8de8\\u6564 GridJsOptions \\u95b0\\u5d87\\u7586\\u9352\\u6d98\\u7f13\\u7f02\\u64b3\\u74e8\\u7039\\u70b0\\u7de5

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### DefaultGridJsJsonCache() {#DefaultGridJsJsonCache--}
```
public DefaultGridJsJsonCache()
```


\\u6d63\\u8de8\\u6564\\u934f\\u3125\\u772c Config \\u95b0\\u5d87\\u7586\\u9352\\u6d98\\u7f13\\u7f02\\u64b3\\u74e8\\u7039\\u70b0\\u7de5\\u951b\\u581f\\u68e4\\u9359\\u509b\\u702f\\u95ab\\u72b2\\u56b1\\u93c1\\u5e2e\\u7d1a

### clearAll() {#clearAll--}
```
public void clearAll()
```


Clear all caches

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
### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public String getCacheKey(String uid, String fileName)
```


Generate a cache key. Customers can decide whether to include the uid based on business requirements. - If only the file name matters: ignore uid and use fileName only (recommended, allows sharing cache across same file). - If distinguishing files with the same name is required: use uid (strict mode).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
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
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public void invalidate(String cacheKey)
```


Invalidate the specified cache entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String |  |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public void invalidateAllForUid(String uid)
```


Invalidate all cache entries containing the specified uid. This is useful when you don't know the exact fileName used for caching.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public void setJson(String cacheKey, String json)
```


Write JSON into cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String |  |
| json | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public String tryGetJson(String cacheKey)
```


Attempt to retrieve JSON from cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String |  |

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

