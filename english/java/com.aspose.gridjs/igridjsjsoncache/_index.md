---
title: IGridJsJsonCache
second_title: Aspose.Cells for Java API Reference
description: JSON cache interface - customers implement specific storage and invalidation strategies
type: docs
url: /java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

JSON cache interface - customers implement specific storage and invalidation strategies
## Methods

| Method | Description |
| --- | --- |
| [clearAll()](#clearAll--) | Clear all caches |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Generate a cache key. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Invalidate the specified cache entry. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Invalidate all cache entries containing the specified uid. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Write JSON into cache. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Attempt to retrieve JSON from cache. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Clear all caches

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Generate a cache key. Customers can decide whether to include the uid based on business requirements. - If only the file name matters: ignore uid and use fileName only (recommended, allows sharing cache across same file). - If distinguishing files with the same name is required: use uid (strict mode).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | Unique identifier of the file (may differ per load) |
| fileName | java.lang.String | Original file name |

**Returns:**
java.lang.String - Cache key
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Invalidate the specified cache entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache key |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Invalidate all cache entries containing the specified uid. This is useful when you don't know the exact fileName used for caching.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | Unique identifier to match in cache keys |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Write JSON into cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache key |
| json | java.lang.String | JSON string |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Attempt to retrieve JSON from cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache key |

**Returns:**
java.lang.String - JSON string if cache hit, null otherwise
