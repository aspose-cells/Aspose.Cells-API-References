---
title: "JsonSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات حفظ المصنف كملف JSON."
type: docs
url: /ar/java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

يمثل خيارات حفظ المصنف كملف JSON.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | ينشئ خيارات لحفظ ملف json. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | يشير إلى ما إذا كان يتم تصدير Excel إلى JSON ككائن دائمًا، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف. |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getExportArea()](#getExportArea--) | يحصل على نطاق التصدير. |
| [getExportAsString()](#getExportAsString--) | يصدّر القيمة النصية للخلايا إلى JSON. |
| [getExportEmptyCells()](#getExportEmptyCells--) | يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | يمثل نوع تصدير الارتباط التشعبي إلى JSON. |
| [getExportNestedStructure()](#getExportNestedStructure--) | يتم تصديره كهيكل JSON هرمي أب-ابن. |
| [getExportStylePool()](#getExportStylePool--) | يشير إلى ما إذا كان يتم تصدير الأنماط بشكل جماعي أو فرديًا لكل خلية. |
| [getIndent()](#getIndent--) | يشير إلى المسافة البادئة. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSchemas()](#getSchemas--) | المخطط الأصلي للـ json لكل ورقة عمل. |
| [getSheetIndexes()](#getSheetIndexes--) | يمثل فهارس الأوراق المصدرة. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getToExcelStruct()](#getToExcelStruct--) | يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hasHeaderRow()](#hasHeaderRow--) | يشير إلى ما إذا كان النطاق يحتوي على صف رأس. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | يشير إلى ما إذا كان يتم تصدير Excel إلى JSON ككائن دائمًا، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | يضبط نطاق التصدير. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | يصدّر القيمة النصية للخلايا إلى JSON. |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null. |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | يمثل نوع تصدير الارتباط التشعبي إلى JSON. |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | يتم تصديره كهيكل JSON هرمي أب-ابن. |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | يشير إلى ما إذا كان يتم تصدير الأنماط بشكل جماعي أو فرديًا لكل خلية. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | يشير إلى ما إذا كان النطاق يحتوي على صف رأس. |
| [setIndent(String value)](#setIndent-java.lang.String-) | يشير إلى المسافة البادئة. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | المخطط الأصلي للـ json لكل ورقة عمل. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | يمثل فهارس الأوراق المصدرة. |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


ينشئ خيارات لحفظ ملف json.

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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


يشير إلى ما إذا كان يتم تصدير Excel إلى JSON ككائن دائمًا، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف.

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
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


يحصل على نطاق التصدير.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


يصدّر القيمة النصية للخلايا إلى JSON.

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null.

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


يمثل نوع تصدير الارتباط التشعبي إلى JSON.

انظر [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

القيمة الافتراضية هي [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


يتم تصديره كهيكل JSON هرمي أب-ابن.

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


يشير إلى ما إذا كان يتم تصدير الأنماط بشكل جماعي أو فرديًا لكل خلية.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


يشير إلى المسافة البادئة.

**Remarks**

إذا كانت المسافة البادئة فارغة أو null، فإن JSON المُصدَّر غير مُنسَّق.

**Returns:**
java.lang.String
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
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


المخطط الأصلي للـ json لكل ورقة عمل.

**Returns:**
java.lang.String[]
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


يمثل فهارس الأوراق المصدرة.

**Returns:**
int[]
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة.

**Returns:**
boolean
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
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel.

**Remarks**

فقط لتحويل النطاق إلى JSON.

**Returns:**
boolean
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
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


يشير إلى ما إذا كان النطاق يحتوي على صف رأس.

**Returns:**
boolean
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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


يشير إلى ما إذا كان يتم تصدير Excel إلى JSON ككائن دائمًا، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


يضبط نطاق التصدير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


يصدّر القيمة النصية للخلايا إلى JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


يمثل نوع تصدير الارتباط التشعبي إلى JSON.

انظر [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

القيمة الافتراضية هي [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


يتم تصديره كهيكل JSON هرمي أب-ابن.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


يشير إلى ما إذا كان يتم تصدير الأنماط بشكل جماعي أو فرديًا لكل خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


يشير إلى ما إذا كان النطاق يحتوي على صف رأس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


يشير إلى المسافة البادئة.

**Remarks**

إذا كانت المسافة البادئة فارغة أو null، فإن JSON المُصدَّر غير مُنسَّق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


المخطط الأصلي للـ json لكل ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


يمثل فهارس الأوراق المصدرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel.

**Remarks**

فقط لتحويل النطاق إلى JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

