---
title: "GridJsWorkbook"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الفئة الرئيسية للدخول لـ GridJs"
type: docs
url: /ar/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

يمثل الفئة الرئيسية للدخول لـ GridJs
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | ينشئ نسخة جديدة من GridJsWorkbook. |
## حقول

| حقل | الوصف |
| --- | --- |
| [CacheImp](#CacheImp) | تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت تريد تخزين الذاكرة المؤقتة بطريقة تدفق، تحتاج إلى ضبطها وتنفيذها. |
| [CalculateEngine](#CalculateEngine) | تنفيذ مخصص لمحرك الحساب، إذا كنت تريد إجراء حساب مخصص، تحتاج إلى ضبطه وتنفيذه. |
| [PICTURE_TYPE](#PICTURE-TYPE) | قيمة const لنوع الصورة |
| [UpdateMonitor](#UpdateMonitor) | الحصول/التعيين لمراقب التحديث لتتبع عملية التحديث |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | ينفّذ (يطبق) جميع عمليات التشويه في المصنف عن طريق إزالة أشكال التشويه وأشكالها المستهدفة أو مسح محتويات نطاق الخلايا المستهدف. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | تحقق مما إذا كانت نسخة دفتر العمل موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق في وضع التعاون فقط. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | نسخ الصورة أو الشكل. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | يحصل على سلسلة رسالة الخطأ بتنسيق JSON. |
| [exportToJson()](#exportToJson--) | يحصل على سلسلة JSON من بيانات الذاكرة، اسم الملف الافتراضي في JSON هو: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | يحصل على دليل الذاكرة المؤقتة لتخزين ملف جدول البيانات. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | يحصل على تنسيق التحميل حسب امتداد الملف |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | احصل على تدفق الصورة. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | يحصل على عنوان URL للصورة. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | يحصل على بيانات مصفوفة البايت للكائن المدمج ole. |
| [getSettings()](#getSettings--) | يمثل إعدادات المصنف. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e ورقة \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | ينشئ معرفًا فريدًا جديدًا لذاكرة التخزين المؤقت للملف باستخدام اسم الملف المعطى. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | يستورد ملف Excel من مسار الملف. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | يستورد ملف Excel من تدفق الملف. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | يستورد ملف Excel من مسار الملف. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | يستورد ملف Excel من مسار الملف وكلمة مرور الفتح. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | يستورد ملف Excel من سلسلة بتنسيق JSON. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | يدرج صورة في ورقة العمل من تدفق الملف أو URL (يجب توفير إما تدفق الملف أو URL) أو يدرج شكلًا عندما يكون p.type أحد AutoShapeType |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | إنشاء JSON من دفتر العمل الموجود في الذاكرة وكتابته إلى التدفق المحدد. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | استرجاع سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، يحدد اسم ملف الإخراج في JSON، ويكتبها إلى التدفق. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | استرجاع سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، وكتابتها إلى التدفق. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | يطبق تحديثًا دفعيًا على بيانات الذاكرة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | ينفذ حذفًا على ملف Excel بناءً على مصفوفة من عمليات JSON. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | يحفظ بيانات الذاكرة إلى ملف الذاكرة المؤقتة باستخدام اسم الملف المحدد ويحدد أيضًا كلمة مرور الفتح، تنسيق الحفظ يعتمد على امتداد الملف لاسم الملف. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | يحفظ بيانات الذاكرة إلى التدفق، بناءً على تنسيق الملف الأصلي. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | يحفظ بيانات الذاكرة إلى مسار الملف، إذا كان للملف امتداد، تنسيق الحفظ يعتمد على امتداد الملف. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | يحفظ بيانات الذاكرة إلى التدفق، تنسيق الحفظ هو html |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | يحفظ بيانات الذاكرة إلى التدفق، تنسيق الحفظ هو pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | يحفظ بيانات الذاكرة إلى sream، تنسيق الحفظ هو xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | يضبط دليل التخزين المؤقت لحفظ ملفات جداول البيانات. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | حدد عنوان URL لإجراء الحصول على الصورة الأساسية من المتحكم. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | يضبط InterruptMonitor لعملية التحميل. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | يضبط InterruptMonitor لعملية الحفظ. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | يمثل إعدادات المصنف. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | يضبط شفافية أشكال الحجب في دفتر العمل. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | ترجمة جميع قيم السلاسل إلى اللغة المستهدفة في ورقة العمل |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | يطبق عملية التحديث. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


ينشئ نسخة جديدة من GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت تريد تخزين الذاكرة المؤقتة بطريقة تدفق، تحتاج إلى ضبطها وتنفيذها.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


تنفيذ مخصص لمحرك الحساب، إذا كنت تريد إجراء حساب مخصص، تحتاج إلى ضبطه وتنفيذه.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


قيمة const لنوع الصورة

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


الحصول/التعيين لمراقب التحديث لتتبع عملية التحديث

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


ينفّذ (يطبق) جميع عمليات التشويه في المصنف عن طريق إزالة أشكال التشويه وأشكالها المستهدفة أو مسح محتويات نطاق الخلايا المستهدف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| excelFilePath | java.lang.String | مسار ملف Excel. |
| uid | java.lang.String | المعرّف الفريد لدفتر العمل. إذا كان null أو فارغًا، سيتم إنشاء uid جديد بناءً على مسار الملف. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


نسخ الصورة أو الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| p | java.lang.String | سلسلة JSON للعملية التي تحدد موقع الخلية، تحتوي على اسم ورقة العمل، الصف العلوي الأيسر، العمود العلوي الأيسر للصورة أو الشكل\\\\u951b\\\\u5b94tc \\{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\\} |

**Returns:**
java.lang.String - سلسلة JSON للصورة المنسوخة الجديدة
### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


يحصل على سلسلة رسالة الخطأ بتنسيق JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| msg | java.lang.String | رسالة الخطأ. |

**Returns:**
java.lang.String - سلسلة JSON.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


يحصل على سلسلة JSON من بيانات الذاكرة، اسم الملف الافتراضي في JSON هو: book1.

**Returns:**
java.lang.String - سلسلة JSON.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1.. |

**Returns:**
java.lang.String - سلسلة JSON.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1.. |

**Returns:**
java.lang.StringBuilder - الـ JSON StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


يحصل على دليل التخزين المؤقت لتخزين ملف جدول البيانات. إذا لم يتم تعيينه، سنستخدم الخاصية الثابتة من [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) أو [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) .

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


يحصل على تنسيق التحميل حسب امتداد الملف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extension | java.lang.String | امتداد الملف، عادةً يبدأ بـ '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


احصل على تدفق الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| picid | java.lang.String | معرف الصورة. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - تدفق الصورة
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


يحصل على عنوان URL للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| picid | java.lang.String | معرف الصورة. |
| delimiter | java.lang.String | فاصل السلسلة. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويضبط اسم ملف الإخراج في JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |

**Returns:**
java.lang.StringBuilder - مُكوّن سلسلة JSON
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


يمثل إعدادات المصنف.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e ورقة \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


ينشئ معرفًا فريدًا جديدًا لذاكرة التخزين المؤقت للملف باستخدام اسم الملف المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


يستورد ملف Excel من تدفق الملف مع تنسيق التحميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filestream | java.io.InputStream | دفق ملف Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). تنسيق التحميل لملف Excel. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filestream | java.io.InputStream | دفق ملف Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). تنسيق التحميل لملف Excel. |
| password | java.lang.String | كلمة المرور المفتوحة لملف Excel. يمكن أن تكون القيمة فارغة إذا لم يتم تعيين كلمة مرور. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


يستورد ملف Excel من مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | المسار الكامل للملف. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


يستورد ملف Excel من تدفق الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرّف الفريد لذاكرة التخزين المؤقت للملف، إذا تم تعيينه إلى فارغ، سيتم إنشاؤه تلقائيًا. |
| filestream | java.io.InputStream | دفق ملف Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). تنسيق التحميل لملف Excel. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرّف الفريد لذاكرة التخزين المؤقت للملف، إذا تم تعيينه إلى فارغ، سيتم إنشاؤه تلقائيًا. |
| filestream | java.io.InputStream | دفق ملف Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). تنسيق التحميل لملف Excel. |
| password | java.lang.String | كلمة المرور المفتوحة لملف Excel. يمكن أن تكون القيمة فارغة إذا لم يتم تعيين كلمة مرور |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


يستورد ملف Excel من مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرّف الفريد لذاكرة التخزين المؤقت للملف، إذا تم تعيينه إلى فارغ، سيتم إنشاؤه تلقائيًا. |
| fileName | java.lang.String | المسار الكامل للملف. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


يستورد ملف Excel من مسار الملف وكلمة مرور الفتح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرّف الفريد لذاكرة التخزين المؤقت للملف، إذا تم تعيينه إلى فارغ، سيتم إنشاؤه تلقائيًا. |
| fileName | java.lang.String | المسار الكامل للملف. |
| password | java.lang.String | كلمة المرور المفتوحة لملف Excel. يمكن أن تكون القيمة فارغة إذا لم يتم تعيين كلمة مرور. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


يستورد ملف Excel من سلسلة بتنسيق JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| json | java.lang.String | سلسلة تنسيق JSON. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


يدرج صورة في ورقة العمل من تدفق الملف أو URL (يجب توفير إما تدفق الملف أو URL) أو يدرج شكلًا عندما يكون p.type أحد AutoShapeType

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرّف الفريد لذاكرة التخزين المؤقت للملف |
| p | java.lang.String | سلسلة تنسيق JSON للعملية التي تحدد موقع الخلية، اسم ورقة العمل، الصف العلوي الأيسر، العمود العلوي الأيسر للصورة\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | دفق ملف الصورة |
| imageUrl | java.lang.String | عنوان URL لملف الصورة |

**Returns:**
java.lang.String - سلسلة تنسيق JSON للصورة المدخلة
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


إنشاء JSON من الـWorkbook الموجود في الذاكرة وكتابته إلى الدفق المحدد. يَخزّن JSON المُنشأ اختياريًا لتسريع الاسترجاع اللاحق. الاختلافات الرئيسية عن JsonToStreamByUid: - يستخدم هذا الأسلوب حالة الـWorkbook الحالية في الذاكرة (حقل wb) - يقوم JsonToStreamByUid بإعادة تحميل الـWorkbook من ملفات ذاكرة التخزين المؤقت .cells على القرص - استخدم هذا الأسلوب عندما تريد تصدير حالة الـWorkbook الحالية بعد التعديلات - استخدم JsonToStreamByUid عندما تحتاج إلى إعادة إنشاء JSON من حالة ملف مخزّن مسبقًا سلوك التخزين المؤقت (عند توفير uid): - يتحقق من ذاكرة التخزين المؤقت لـJSON قبل الإنشاء (الذاكرة L1 + القرص L2) - إذا لم توجد نسخة مخزّنة، ينشئ JSON من الـWorkbook في الذاكرة - يخزن JSON المُنشأ في الذاكرة المؤقتة للطلبات المستقبلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الإخراج لكتابة بيانات JSON إليه |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| اسم الملف | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


استرجاع سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، يحدد اسم ملف الإخراج في JSON، ويكتبها إلى التدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| sheetName | java.lang.String | اسم الورقة. |

**Returns:**
java.lang.StringBuilder - مُكوّن سلسلة JSON
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


استرجاع سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، وكتابتها إلى التدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | التدفق الذي سيتم كتابته |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| sheetName | java.lang.String | اسم الورقة. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


يطبق تحديثًا دفعيًا على بيانات الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| json | java.lang.String | سلسلة تنسيق JSON للتحديث. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


ينفذ حذفًا على ملف Excel بناءً على مصفوفة من عمليات JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| excelFilePath | java.lang.String | مسار ملف Excel المراد تنقيحه. |
| uid | java.lang.String | المعرّف الفريد لدفتر العمل. إذا كان null أو فارغًا، سيتم إنشاء uid جديد بناءً على مسار الملف. |
| arrayOfRedactionOpr | java.lang.String[] | مصفوفة من سلاسل JSON تمثل عمليات التنقيح التي سيتم تطبيقها. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


يحفظ بيانات الذاكرة إلى ملف الذاكرة المؤقتة باستخدام اسم الملف المحدد ويحدد أيضًا كلمة مرور الفتح، تنسيق الحفظ يعتمد على امتداد الملف لاسم الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |
| اسم الملف | java.lang.String | اسم الملف لحفظه. |
| password | java.lang.String | كلمة مرور فتح ملف Excel. يمكن أن تكون القيمة فارغة إذا لم يتم تعيين كلمة مرور. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


يحفظ بيانات الذاكرة إلى التدفق، بناءً على تنسيق الملف الأصلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق لحفظه. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


يحفظ بيانات الذاكرة إلى مسار الملف، إذا كان للملف امتداد، تنسيق الحفظ يعتمد على امتداد الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار الملف لحفظه. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


يحفظ بيانات الذاكرة إلى التدفق، تنسيق الحفظ هو html

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق لحفظه. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار الملف لحفظه. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


يحفظ بيانات الذاكرة إلى التدفق، تنسيق الحفظ هو pdf.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق لحفظه. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو pdf.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار الملف لحفظه. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


يحفظ بيانات الذاكرة إلى sream، تنسيق الحفظ هو xlsx.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | الدفق لحفظه. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو xlsx.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | java.lang.String | مسار الملف لحفظه. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


يضبط دليل التخزين المؤقت لتخزين ملف جدول البيانات. إذا لم يتم تعيينه، سنستخدم الخاصية الثابتة من [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) أو [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


حدد عنوان URL لإجراء الحصول على الصورة الأساسية من المتحكم.

**Remarks**

عند كون CacheImp فارغًا، نحتاج إلى تعيين هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| baseImageURL | java.lang.String | عنوان URL لإجراء الحصول على الصورة الأساسية. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


يضبط InterruptMonitor لعملية التحميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | مثيل InterruptMonitor. |
| calculateTimeoutMilliseconds | int | مهلة التحميل بالمللي ثانية للملف. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


يضبط InterruptMonitor لعملية الحفظ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | مثيل InterruptMonitor. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


يمثل إعدادات المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


يضبط شفافية أشكال الحجب في دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| excelFilePath | java.lang.String | مسار ملف Excel. |
| uid | java.lang.String | المعرّف الفريد لدفتر العمل. إذا كان null أو فارغًا، سيتم إنشاء uid جديد بناءً على مسار الملف. |
| isTransparent | boolean | إذا كان true، يضبط الشفافية إلى 0.89 (شفافة جزئيًا)؛ إذا كان false، يضبط الشفافية إلى 1 (غير شفافة/غير مرئية). |

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
java.lang.String - سلسلة تنسيق JSON لنتيجة التحديث.
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

