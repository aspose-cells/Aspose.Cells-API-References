---
title: "IGridJsJsonCache"
second_title: "Aspose.Cells for Java API 参考"
description: "JSON 缓存接口 - 客户实现特定的存储和失效策略"
type: docs
url: /zh/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

JSON 缓存接口 - 客户实现特定的存储和失效策略
## 方法

| 方法 | 描述 |
| --- | --- |
| [clearAll()](#clearAll--) | 清除所有缓存 |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | 生成缓存键。 |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | 使指定的缓存条目失效。 |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | 使包含指定 uid 的所有缓存条目失效。 |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | 将 JSON 写入缓存。 |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | 尝试从缓存中检索 JSON。 |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


清除所有缓存

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


生成缓存键。客户可以根据业务需求决定是否包含 uid。- 如果仅文件名重要：忽略 uid，仅使用 fileName（推荐，允许在相同文件之间共享缓存）。- 如果需要区分同名文件：使用 uid（严格模式）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 文件的唯一标识符（每次加载可能不同） |
| fileName | java.lang.String | 原始文件名 |

**Returns:**
java.lang.String - 缓存键
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


使指定的缓存条目失效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cacheKey | java.lang.String | 缓存键 |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


使包含指定 uid 的所有缓存条目失效。当您不知道用于缓存的确切 fileName 时，这很有用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | java.lang.String | 用于匹配缓存键的唯一标识符 |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


将 JSON 写入缓存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cacheKey | java.lang.String | 缓存键 |
| json | java.lang.String | JSON 字符串 |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


尝试从缓存中检索 JSON。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cacheKey | java.lang.String | 缓存键 |

**Returns:**
java.lang.String - 如果缓存命中则为 JSON 字符串，否则为 null
