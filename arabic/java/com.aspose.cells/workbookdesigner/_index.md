---
title: "WorkbookDesigner"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل جدول بيانات المصمم."
type: docs
url: /ar/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

يغلف الكائن الذي يمثل جدول بيانات المصمم.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | يمسح جميع مصادر البيانات. |
| [containsVariables()](#containsVariables--) | يشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | يشير إلى ما إذا كان يجب حساب الصيغ. |
| [getCallBack()](#getCallBack--) | يحصل على واجهة الاستدعاء لمعالجة smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | يشير إلى ما إذا كان الرأس/التذييل يحتوي على علامات ذكية ويجب معالجتهما معًا. |
| [getLineByLine()](#getLineByLine--) | يشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي. |
| [getSmartMarkers()](#getSmartMarkers--) | يعيد مجموعة من العلامات الذكية في جدول بيانات. |
| [getSortDataSource()](#getSortDataSource--) | يشير إلى ما إذا كان مصدر البيانات يتم فرزه. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة \"\"؛ |
| [getUpdateReference()](#getUpdateReference--) | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | يحصل على اسم ورقة العمل التي تحتوي على متغيرات العلامة الذكية. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) . |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [process(boolean isPreserved)](#process-boolean-) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | يعالج العلامات الذكية ويملأ قيم مصدر البيانات. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | يشير إلى ما إذا كان يجب حساب الصيغ. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | يضبط واجهة الاستدعاء العكسي لمعالجة العلامة الذكية. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | يشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | يضبط مصدر البيانات لكائن [ICellsDataTable](../../com.aspose.cells/icellsdatatable). |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | يضبط ربط البيانات بمتغير. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | اضبط مصدر البيانات. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | اضبط مصدر البيانات. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | اضبط مصدر البيانات. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | يشير إلى ما إذا كان الرأس/التذييل يحتوي على علامات ذكية ويجب معالجتهما معًا. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | اضبط قيمة سلسلة JSON كمصدر بيانات للعلامات الذكية. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | يشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | يشير إلى ما إذا كان مصدر البيانات يتم فرزه. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة \"\"؛ |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | يضبط اسم ورقة العمل التي تحتوي على متغيرات العلامة الذكية. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | يضبط كائن [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


يقوم بتهيئة نسخة جديدة من الفئة [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | ملف دفتر العمل النموذجي. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


يمسح جميع مصادر البيانات.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


يشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية WorkbookDesigner.VariablesWorksheetName. سيتم إزالة هذه الخاصية بعد 3 أشهر اعتبارًا من سبتمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


يشير إلى ما إذا كان يجب حساب الصيغ.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


يحصل على واجهة الاستدعاء لمعالجة smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


يشير إلى ما إذا كان الرأس/التذييل يحتوي على علامات ذكية ويجب معالجتهما معًا.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


يشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر.

**Remarks**

ملاحظة: هذه الفئة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام علامات ذكية للنطاق. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


يعيد مجموعة من العلامات الذكية في جدول بيانات.

**Remarks**

يتم إنشاء مصفوفة سلاسل نصية في كل استدعاء. يتم فرز المصفوفة وإزالة القيم المكررة.

**Returns:**
java.lang.String[] - مجموعة من العلامات الذكية
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


يشير إلى ما إذا كان مصدر البيانات يتم فرزه.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أكتوبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. سيتم فرز مصدر بيانات JSON إذا كانت العلامة الذكية تحتوي على معلمات تصاعدية وتنازلية.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة \"\"؛

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


يحصل على اسم ورقة العمل التي تحتوي على متغيرات العلامة الذكية.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


يحصل على كائن [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) .

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isPreserved | boolean | True إذا تم حفظ العلامة الذكية غير المعروفة. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

**Remarks**

ملاحظة: هذه الفئة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام علامات ذكية للنطاق. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق المراد معالجته |
| isPreserved | boolean | True إذا تم حفظ العلامة الذكية غير المعروفة. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

**Remarks**

هذه الطريقة تعمل على مستوى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس ورقة العمل. |
| isPreserved | boolean | True إذا تم حفظ العلامة الذكية غير المعروفة. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


يشير إلى ما إذا كان يجب حساب الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


يضبط واجهة الاستدعاء العكسي لمعالجة العلامة الذكية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


يشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية WorkbookDesigner.VariablesWorksheetName. سيتم إزالة هذه الخاصية بعد 3 أشهر اعتبارًا من سبتمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


يضبط مصدر البيانات لكائن [ICellsDataTable](../../com.aspose.cells/icellsdatatable).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصدر البيانات | java.lang.String | اسم مصدر البيانات. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | جدول البيانات. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


يضبط ربط البيانات بمتغير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| متغير | java.lang.String | اسم المتغير الذي تم إنشاؤه باستخدام العلامة الذكية. |
| بيانات | java.lang.Object | بيانات المصدر. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


اضبط مصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصدر البيانات | java.lang.String | اسم مصدر البيانات. |
| rs | java.sql.ResultSet | مجموعة النتائج. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


اضبط مصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصدر البيانات | java.lang.String | اسم مصدر البيانات. |
| rs | java.sql.ResultSet | مجموعة النتائج. |
| عدد الصفوف | int | عدد البيانات لمجموعة النتائج المعطاة. يجب أن يكون عدد الصفوف الدقيق أو -1؛ إذا كانت مجموعة النتائج للأمام فقط، يجب على المستخدم إعطاء عدد الصفوف الدقيق هنا، وإلا قد لا يتم معالجة العلامة الذكية بشكل صحيح عندما لا يتم تعيين \"noadd\" للعلامة الذكية. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


اضبط مصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rs | java.sql.ResultSet | مجموعة النتائج. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


يشير إلى ما إذا كان الرأس/التذييل يحتوي على علامات ذكية ويجب معالجتهما معًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


اضبط قيمة سلسلة JSON كمصدر بيانات للعلامات الذكية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الجدول. إذا كانت قيمة JSON تمثل كائنًا، قد تكون فارغة. |
| json | java.lang.String | قيمة سلسلة JSON. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


يشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر.

**Remarks**

ملاحظة: هذه الفئة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام علامات ذكية للنطاق. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


يشير إلى ما إذا كان مصدر البيانات يتم فرزه.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أكتوبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. سيتم فرز مصدر بيانات JSON إذا كانت العلامة الذكية تحتوي على معلمات تصاعدية وتنازلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة \"\"؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


يضبط اسم ورقة العمل التي تحتوي على متغيرات العلامة الذكية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


يضبط كائن [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

