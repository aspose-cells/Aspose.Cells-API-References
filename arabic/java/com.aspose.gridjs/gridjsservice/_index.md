---
title: "GridJsService"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر واجهات برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم."
type: docs
url: /ar/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

يوفر واجهات برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | البناء الافتراضي لـ GridJsService |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | يطبق عملية إضافة صورة من ملف محلي. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | يطبق عملية إضافة صورة من ملف محلي. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | تحقق مما إذا كانت نسخة دفتر العمل موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق في وضع التعاون فقط. |
| [clearAllJsonCache()](#clearAllJsonCache--) | يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON (الذاكرة والقرص). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON المرتبطة بالمعرف الفريد المحدد. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | يطبق عملية نسخ الصورة. |
| [destroy()](#destroy--) | هذه الطريقة مخصصة لجافا فقط، تنفذ طريقة destroy في DisposableBean، والتي سيتم استدعاؤها تلقائيًا بواسطة Spring عند انتهاء الطلب، في الواقع ستستدعي طريقة Dispose. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للملف بواسطة المعرف الفريد المحدد. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | يكتب سلسلة JSON للملف إلى الدفق. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | يكتب سلسلة JSON للملف إلى الدفق باستخدام المعرف الفريد المحدد. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | يطبق عملية تنزيل الملف |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | احصل على تدفق الملف |
| [getSettings()](#getSettings--) | يمثل إعدادات المصنف. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | احصل على تدفق الصورة. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | يحصل على عنوان URL للصورة. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | يكتب سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد إلى التدفق.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | يحصل على بيانات مصفوفة البايت للكائن المدمج ole. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | يمثل إعدادات المصنف. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | ترجمة جميع قيم السلاسل إلى اللغة المستهدفة في ورقة العمل |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | يطبق عملية التحديث. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


البناء الافتراضي لـ GridJsService

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
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
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


يطبق عملية إضافة صورة من ملف محلي.

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
public boolean checkInCacheForCollaborative(String uid)
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
public void clearAllJsonCache()
```


يمسح جميع إدخالات ذاكرة التخزين المؤقت لـ JSON (الذاكرة والقرص).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


يمسح جميع إدخالات ذاكرة JSON المؤقتة التابعة للمعرف الفريد المحدد. استدعِ هذا بعد تعديل ملف المصدر خارج النطاق حتى يُعيد الطلب التالي توليد JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


يطبق عملية نسخ الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | معامل سلسلة JSON |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.String - نتيجة سلسلة JSON
### destroy() {#destroy--}
```
public void destroy()
```


هذه الطريقة مخصصة لجافا فقط، تنفذ طريقة destroy في DisposableBean، والتي سيتم استدعاؤها تلقائيًا بواسطة Spring عند انتهاء الطلب، في الواقع ستستدعي طريقة Dispose.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


يحصل على سلسلة JSON للملف بواسطة المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف الكامل |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


يكتب سلسلة JSON للملف إلى الدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| filePath | java.lang.String | مسار الملف الكامل |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


يكتب سلسلة JSON للملف إلى الدفق باستخدام المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| filePath | java.lang.String | مسار الملف الكامل |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
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
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


احصل على تدفق الملف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileid | java.lang.String | معرف الملف |

**Returns:**
java.io.InputStream - تدفق الملف
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


يمثل إعدادات المصنف.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
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
public String imageUrl(String baseURL, String picid, String uid)
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
public StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public String load(String uid, String filename)
```


يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |

**Returns:**
java.lang.String - سلسلة JSON
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
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
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


يمثل إعدادات المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


ترجمة جميع قيم السلاسل إلى اللغة المستهدفة في ورقة العمل

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| sheetName | java.lang.String | اسم الورقة |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | المترجم الذي يُنفّذ وظيفة الترجمة |
| لغة الهدف | java.lang.String | اللغة المستهدفة |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


يطبق عملية التحديث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| p | java.lang.String | سلسلة تنسيق JSON لعملية التحديث. |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

