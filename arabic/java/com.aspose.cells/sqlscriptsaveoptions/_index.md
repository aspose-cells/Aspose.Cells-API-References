---
title: "SqlScriptSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات حفظ sql."
type: docs
url: /ar/java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

يمثل خيارات حفظ sql.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | ينشئ خيارات لحفظ ملف sql. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | أدرج سطرًا فارغًا بين كل بيانات. |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getColumnTypeMap()](#getColumnTypeMap--) | يحصل على خريطة نوع العمود لمختلف قواعد البيانات. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getCreateTable()](#getCreateTable--) | يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getExportArea()](#getExportArea--) | يحصل على نطاق التصدير. |
| [getExportAsString()](#getExportAsString--) | يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية. |
| [getIdName()](#getIdName--) | يحصل على اسم عمود المعرف. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getOperatorType()](#getOperatorType--) | يحصل على نوع المشغل للـ sql. |
| [getPrimaryKey()](#getPrimaryKey--) | يمثل العمود الذي هو المفتاح الأساسي لجدول البيانات. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSeparator()](#getSeparator--) | يحصل على فاصل الأحرف لسكريبت sql. |
| [getSheetIndexes()](#getSheetIndexes--) | يمثل فهارس الأوراق المصدرة. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getStartId()](#getStartId--) | يحصل على معرف البداية. |
| [getTableName()](#getTableName--) | يحصل على اسم الجدول. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hasHeaderRow()](#hasHeaderRow--) | يشير إلى ما إذا كان النطاق يحتوي على صف رأس. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | أدرج سطرًا فارغًا بين كل بيانات. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | يضبط خريطة نوع العمود لمختلف قواعد البيانات. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | يضبط نطاق التصدير. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | يشير إلى ما إذا كان النطاق يحتوي على صف رأس. |
| [setIdName(String value)](#setIdName-java.lang.String-) | يضبط اسم عمود المعرف. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setOperatorType(int value)](#setOperatorType-int-) | يضبط نوع المشغل للـ sql. |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | يمثل العمود الذي هو المفتاح الأساسي لجدول البيانات. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setSeparator(char value)](#setSeparator-char-) | يضبط فاصل الأحرف لسكريبت sql. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | يمثل فهارس الأوراق المصدرة. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setStartId(int value)](#setStartId-int-) | يضبط معرف البداية. |
| [setTableName(String value)](#setTableName-java.lang.String-) | يضبط اسم الجدول. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


ينشئ خيارات لحفظ ملف sql.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


أدرج سطرًا فارغًا بين كل بيانات.

**Remarks**

إذا كان [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) هو '\\n' ، فمن الأفضل ضبط هذه الخاصية كقيمة true لزيادة قابلية القراءة.

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
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة.

**Remarks**

القيمة الافتراضية هي false، نحن نتحقق فقط من الصف الأول للأداء. إذا كانت هذه الخاصية true وكانت الأعمدة تحتوي على أنواع قيم مختلطة، فسيكون نوع الأعمدة نصًا.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء.

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
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


يحصل على خريطة نوع العمود لمختلف قواعد البيانات.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول.

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


يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


يحصل على اسم عمود المعرف.

**Remarks**

إذا تم ضبط هذه الخاصية، سيتم إدراج عمود بقيمة int تتزايد تلقائيًا.

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
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


يحصل على نوع المشغل للـ sql.

انظر [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


يمثل العمود الذي هو المفتاح الأساسي لجدول البيانات.

**Returns:**
int
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


يحصل على فاصل الأحرف لسكريبت sql.

**Remarks**

يمكن أن يكون فقط ' ' أو '\\n'. إذا كان

**Returns:**
char
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


يمثل فهارس الأوراق المصدرة.

**Returns:**
int[]
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
### getStartId() {#getStartId--}
```
public int getStartId()
```


يحصل على معرف البداية.

**Remarks**

يعمل فقط عندما يتم تعيين [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--).

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


يحصل على اسم الجدول.

**Returns:**
java.lang.String
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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


أدرج سطرًا فارغًا بين كل بيانات.

**Remarks**

إذا كان [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) هو '\\n' ، فمن الأفضل ضبط هذه الخاصية كقيمة true لزيادة قابلية القراءة.

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

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة.

**Remarks**

القيمة الافتراضية هي false، نحن نتحقق فقط من الصف الأول للأداء. إذا كانت هذه الخاصية true وكانت الأعمدة تحتوي على أنواع قيم مختلطة، فسيكون نوع الأعمدة نصًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء.

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

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


يضبط خريطة نوع العمود لمختلف قواعد البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

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

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول.

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


يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية.

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

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


يضبط اسم عمود المعرف.

**Remarks**

إذا تم ضبط هذه الخاصية، سيتم إدراج عمود بقيمة int تتزايد تلقائيًا.

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

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


يضبط نوع المشغل للـ sql.

انظر [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


يمثل العمود الذي هو المفتاح الأساسي لجدول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


يضبط فاصل الأحرف لسكريبت sql.

**Remarks**

يمكن أن يكون فقط ' ' أو '\\n'. إذا كان

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


يمثل فهارس الأوراق المصدرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] |  |

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

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


يضبط معرف البداية.

**Remarks**

يعمل فقط عندما يتم تعيين [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


يضبط اسم الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

