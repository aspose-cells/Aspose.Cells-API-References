---
title: "IGridJsJsonCache"
second_title: "Aspose.Cells for Java API Reference"
description: "واجهة تخزين JSON المؤقت - يقوم العملاء بتنفيذ استراتيجيات التخزين والإبطال المحددة."
type: docs
url: /ar/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

واجهة تخزين JSON المؤقت - يقوم العملاء بتنفيذ استراتيجيات التخزين والإبطال المحددة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clearAll()](#clearAll--) | مسح جميع الذاكرات المؤقتة |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | إنشاء مفتاح ذاكرة مؤقتة. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | إبطال الإدخال المحدد في الذاكرة المؤقتة. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | إبطال جميع إدخالات الذاكرة المؤقتة التي تحتوي على المعرف المحدد. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | اكتب JSON في الذاكرة المؤقتة. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | حاول استرجاع JSON من الذاكرة المؤقتة. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


مسح جميع الذاكرات المؤقتة

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


إنشاء مفتاح ذاكرة مؤقتة. يمكن للعملاء اتخاذ قرار بشأن تضمين الـ uid بناءً على متطلبات العمل. - إذا كان اسم الملف فقط هو المهم: تجاهل الـ uid واستخدام fileName فقط (مُوصى به، يسمح بمشاركة الذاكرة المؤقتة عبر نفس الملف). - إذا كان التمييز بين الملفات ذات الاسم نفسه مطلوبًا: استخدم uid (وضع صارم).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | معرف فريد للملف (قد يختلف حسب التحميل). |
| fileName | java.lang.String | اسم الملف الأصلي |

**Returns:**
java.lang.String - مفتاح الذاكرة المؤقتة
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


إبطال الإدخال المحدد في الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cacheKey | java.lang.String | مفتاح الذاكرة المؤقتة |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


إبطال جميع إدخالات الذاكرة المؤقتة التي تحتوي على المعرف uid المحدد. هذا مفيد عندما لا تعرف اسم الملف fileName الدقيق المستخدم للتخزين المؤقت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | معرف فريد للمطابقة في مفاتيح الذاكرة المؤقتة |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


اكتب JSON في الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cacheKey | java.lang.String | مفتاح الذاكرة المؤقتة |
| json | java.lang.String | سلسلة JSON |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


حاول استرجاع JSON من الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cacheKey | java.lang.String | مفتاح الذاكرة المؤقتة |

**Returns:**
java.lang.String - سلسلة JSON إذا تم العثور في الذاكرة المؤقتة، وإلا null
