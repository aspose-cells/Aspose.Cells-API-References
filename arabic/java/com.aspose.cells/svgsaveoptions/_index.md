---
title: "SvgSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات حفظ Svg."
type: docs
url: /ar/java/com.aspose.cells/svgsaveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)، [com.aspose.cells.ImageSaveOptions](../../com.aspose.cells/imagesaveoptions)
```
public class SvgSaveOptions extends ImageSaveOptions
```

يمثل خيارات حفظ Svg. للاستخدام المتقدم، يرجى استخدام [WorkbookRender](../../com.aspose.cells/workbookrender) أو [SheetRender](../../com.aspose.cells/sheetrender).

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام فئة ImageSaveOptions. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SvgSaveOptions()](#SvgSaveOptions--) | ينشئ الخيارات لحفظ ملف svg. |
| [SvgSaveOptions(int saveFormat)](#SvgSaveOptions-int-) | ينشئ الخيارات لحفظ ملف svg. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getImageOrPrintOptions()](#getImageOrPrintOptions--) | خيارات إضافية لإنشاء الصورة. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSheetIndex()](#getSheetIndex--) | يحصل على الورقة التي يجب تصديرها. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getStreamProvider()](#getStreamProvider--) | يحصل على IStreamProvider لتصدير الكائنات. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | يضبط الورقة التي يجب تصديرها. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | يضبط IStreamProvider لتصدير الكائنات. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgSaveOptions() {#SvgSaveOptions--}
```
public SvgSaveOptions()
```


ينشئ الخيارات لحفظ ملف svg.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام فئة ImageSaveOptions. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### SvgSaveOptions(int saveFormat) {#SvgSaveOptions-int-}
```
public SvgSaveOptions(int saveFormat)
```


ينشئ الخيارات لحفظ ملف svg.

**Remarks**

ملاحظة: هذا المُنشئ الآن مهجور. بدلاً من ذلك، يرجى استخدام مُنشئ SvgSaveOptions(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الملف. يجب أن يكون svg. |

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Returns:**
boolean
### getImageOrPrintOptions() {#getImageOrPrintOptions--}
```
public ImageOrPrintOptions getImageOrPrintOptions()
```


خيارات إضافية لإنشاء الصورة.

**Remarks**

للاستخدام المتقدم، يرجى استخدام [WorkbookRender](../../com.aspose.cells/workbookrender) أو [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على صيغة حفظ الملف.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


يحصل على الورقة التي يجب تصديرها. إذا كانت القيمة -1، سيتم تصدير الورقة النشطة.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام فئة ImageSaveOptions. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


يحصل على IStreamProvider لتصدير الكائنات.

**Remarks**

إذا تم الحفظ كـ Tiff، يتم تجاهل هذه الخاصية. وإلا، إذا كان يجب حفظ أكثر من صورة واحدة، سنكتب الصور الأخرى باستخدام هذه الخاصية. للاستخدام المتقدم، يرجى استخدام [WorkbookRender](../../com.aspose.cells/workbookrender) أو [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


يحصل على رد النداء للتحذير.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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




### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


يضبط أي ورقة عمل يجب تصديرها. إذا كانت القيمة -1، سيتم تصدير ورقة العمل النشطة.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام فئة ImageSaveOptions. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


يضبط IStreamProvider لتصدير الكائنات.

**Remarks**

إذا تم الحفظ كـ Tiff، يتم تجاهل هذه الخاصية. وإلا، إذا كان يجب حفظ أكثر من صورة واحدة، سنكتب الصور الأخرى باستخدام هذه الخاصية. للاستخدام المتقدم، يرجى استخدام [WorkbookRender](../../com.aspose.cells/workbookrender) أو [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


يضبط رد النداء للتحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

