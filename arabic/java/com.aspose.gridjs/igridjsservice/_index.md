---
title: "IGridJsService"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل واجهة برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم."
type: docs
url: /ar/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

يمثل واجهة برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | يطبق عملية إضافة صورة من ملف محلي. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | يطبق عملية إضافة صورة من عنوان URL بعيد. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | تحقق مما إذا كانت نسخة دفتر العمل موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق في وضع التعاون فقط. |
| [clearAllJsonCache()](#clearAllJsonCache--) | يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON (الذاكرة والقرص). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON المرتبطة بالمعرف الفريد المحدد. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | يطبق عملية نسخ الصورة. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للملف بواسطة المعرف الفريد المحدد. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | اكتب سلسلة JSON للدفتر إلى الدفق |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | يكتب سلسلة JSON للملف إلى الدفق باستخدام المعرف الفريد المحدد. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | يطبق عملية تنزيل الملف |
| [getFile(String fileid)](#getFile-java.lang.String-) | احصل على تدفق الملف |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | احصل على تدفق الصورة. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | يحصل على عنوان URL للصورة. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | يكتب سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد إلى التدفق.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | يحصل على بيانات مصفوفة البايت للكائن المدمج ole. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | يطبق عملية التحديث. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
```


يطبق عملية إضافة صورة من ملف محلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | معامل سلسلة JSON |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| filestream | java.io.InputStream | تدفق الملف للصورة |

**Returns:**
java.lang.String - نتيجة سلسلة JSON
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


يطبق عملية إضافة صورة من عنوان URL بعيد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | معامل سلسلة JSON |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| filestream | java.io.InputStream | تدفق الملف للصورة |
| imageurl | java.lang.String | حدد عنوان URL للصورة. |

**Returns:**
java.lang.String - نتيجة سلسلة JSON
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public abstract boolean checkInCacheForCollaborative(String uid)
```


تحقق مما إذا كانت نسخة دفتر العمل موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق في وضع التعاون فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public abstract void clearAllJsonCache()
```


يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON (الذاكرة والقرص).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


يمسح جميع إدخالات ذاكرة JSON المؤقتة التابعة للمعرف الفريد المحدد. استدعِ هذا بعد تعديل ملف المصدر خارج النطاق حتى يُعيد الطلب التالي توليد JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


يطبق عملية نسخ الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | معامل سلسلة JSON |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.String - نتيجة سلسلة JSON
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


يحصل على سلسلة JSON للملف بواسطة المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


اكتب سلسلة JSON للدفتر إلى الدفق

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| filePath | java.lang.String | مسار الملف |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


يكتب سلسلة JSON للملف إلى الدفق باستخدام المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| filePath | java.lang.String | مسار الملف |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
```


يطبق عملية تنزيل الملف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | معامل JSON |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | اسم الملف |

**Returns:**
java.lang.String - عنوان URL للملف
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


احصل على تدفق الملف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileid | java.lang.String | معرف الملف |

**Returns:**
java.io.InputStream - تدفق الملف
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
```


احصل على تدفق الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| picid | java.lang.String | معرف الصورة. |

**Returns:**
java.io.InputStream - تدفق الصورة
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String imageUrl(String baseURL, String picid, String uid)
```


يحصل على عنوان URL للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseURL | java.lang.String | عنوان URL الأساسي للإجراء. |
| picid | java.lang.String | معرف الصورة. |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.String - عنوان URL للصورة
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
```


يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم الورقة. |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


يكتب سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد إلى التدفق..

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| sheetName | java.lang.String | اسم الورقة. |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public abstract String load(String uid, String filename)
```


يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |

**Returns:**
java.lang.String - سلسلة JSON
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
```


يحصل على بيانات مصفوفة البايت للكائن المدمج ole.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| sheetname | java.lang.String | اسم ورقة العمل. |
| oleid | int | المعرّف للكائن المدمج ole. |
| label | java.lang.String | التسمية المعروضة للكائن المدمج ole. |

**Returns:**
byte[] - بيانات مصفوفة البايت للكائن المدمج ole.
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


يطبق عملية التحديث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | سلسلة تنسيق JSON لعملية التحديث. |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.String
