---
title: "ImportTableOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات استيراد البيانات إلى الخلايا."
type: docs
url: /ar/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

يمثل خيارات استيراد البيانات إلى الخلايا.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | ينشئ خيارات الاستيراد الافتراضية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | يشير إلى ما إذا كان يتم فحص الخلايا المدمجة. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | يحصل على الأعمدة (مؤشرها 0) لاستيرادها من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة. |
| [getConvertGridStyle()](#getConvertGridStyle--) | يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا. |
| [getConvertNumericData()](#getConvertNumericData--) | يحصل على قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية. |
| [getDateFormat()](#getDateFormat--) | يحصل على سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة. |
| [getDefaultValues()](#getDefaultValues--) | القيمة الافتراضية للعنصر في الجدول هي null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل. |
| [getInsertRows()](#getInsertRows--) | يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات. |
| [getNumberFormats()](#getNumberFormats--) | يحصل على تنسيقات الأرقام. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف. |
| [getStyles()](#getStyles--) | يحصل على الأنماط لكل عمود في الجدول. |
| [getTotalColumns()](#getTotalColumns--) | يحصل على إجمالي عدد الأعمدة لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [getTotalRows()](#getTotalRows--) | يحصل على إجمالي عدد الصفوف لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | يشير إلى ما إذا كان يجب استيراد اسم الحقل. |
| [isFormulas()](#isFormulas--) | يشير إلى ما إذا كانت البيانات صيغًا. |
| [isHtmlString()](#isHtmlString--) | يشير إلى ما إذا كانت القيمة تحتوي على وسوم html. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | يشير إلى ما إذا كان يتم فحص الخلايا المدمجة. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | يضبط الأعمدة (بدءًا من الصفر) لاستيرادها من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | القيمة الافتراضية للعنصر في الجدول هي null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل. |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | يشير إلى ما إذا كان يجب استيراد اسم الحقل. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | يشير إلى ما إذا كانت البيانات صيغًا. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | يشير إلى ما إذا كانت القيمة تحتوي على وسوم html. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | يضبط تنسيقات الأرقام |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | يضبط الأنماط لكل عمود في الجدول. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | يضبط العدد الإجمالي للأعمدة لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [setTotalRows(int value)](#setTotalRows-int-) | يضبط العدد الإجمالي للصفوف لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


ينشئ خيارات الاستيراد الافتراضية.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


يشير إلى ما إذا كان يتم فحص الخلايا المدمجة.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


يحصل على الأعمدة (مؤشرها 0) لاستيرادها من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


يحصل على سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


القيمة الافتراضية للعنصر في الجدول هي null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل.

**Remarks**

يعمل فقط مع DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


يحصل على تنسيقات الأرقام.

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


يحصل على الأنماط لكل عمود في الجدول.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


يحصل على إجمالي عدد الأعمدة لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


يحصل على إجمالي عدد الصفوف لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


يشير إلى ما إذا كان يجب استيراد اسم الحقل.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


يشير إلى ما إذا كانت البيانات صيغًا.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


يشير إلى ما إذا كانت القيمة تحتوي على وسوم html.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


يشير إلى ما إذا كان يتم فحص الخلايا المدمجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


يضبط الأعمدة (بدءًا من الصفر) لاستيرادها من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ ووقت مستوردة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


القيمة الافتراضية للعنصر في الجدول هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل.

**Remarks**

يعمل فقط مع DataTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


يشير إلى ما إذا كان يجب استيراد اسم الحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


يشير إلى ما إذا كانت البيانات صيغًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


يشير إلى ما إذا كانت القيمة تحتوي على وسوم html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


يضبط تنسيقات الأرقام

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


يضبط الأنماط لكل عمود في الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


يضبط العدد الإجمالي للأعمدة لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


يضبط العدد الإجمالي للصفوف لاستيرادها من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

