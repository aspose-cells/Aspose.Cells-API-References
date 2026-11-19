---
title: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ GlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المعرفة مسبقًا."
type: docs
url: /ar/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

تنفيذ GlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المعرفة مسبقًا.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | يحصل على اسم التسمية "(All)" في PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | يحصل على قيمة السلسلة المعروضة لقيمة منطقية للخلية |
| [getChartSettings()](#getChartSettings--) | يحصل على إعدادات العولمة للمخطط. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | يحوّل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | يحصل على اسم التسمية "Column Labels" في PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | يحصل على اسم رأس حقل منطقة القيمة في PivotTable. |
| [getDefaultSheetName()](#getDefaultSheetName--) | يحصل على اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا. |
| [getEmptyDataName()](#getEmptyDataName--) | يحصل على اسم التسمية "(blank)" في PivotTable. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | يحصل على قيمة السلسلة المعروضة لقيمة الخطأ في الخلية |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | يحصل على اسم الإجمالي الكلي للدالة. |
| [getListSeparator()](#getListSeparator--) | يحصل على الفاصل للقائمة، ومعلمات الدالة، ...إلخ. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | يحصل على النص المعتمد على الإعدادات الإقليمية للاسم المدمج وفقًا للنص القياسي المعطى. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | يحصل على اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [getMultipleItemsName()](#getMultipleItemsName--) | يحصل على اسم التسمية "(Multiple Items)" في PivotTable. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | يحصل على اسم التسمية "Grand Total" في PivotTable. |
| [getPivotSettings()](#getPivotSettings--) | يحصل على إعدادات العولمة لجدول PivotTable. |
| [getPivotTotalName()](#getPivotTotalName--) | يحصل على اسم التسمية "Total" في PivotTable. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | يحصل على اسم الحماية في PivotTable. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | يحصل على اسم التسمية "Row Labels" في PivotTable. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | يحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على الإعدادات الإقليمية المعطى. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | يحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعدادات الإقليمية المعطى. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | يحصل على اسم نمط الخط الإنجليزي القياسي (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط الإقليمي المعطى. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | يحصل على اسم نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في PivotTable. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| [getTotalName(int functionType)](#getTotalName-int-) | يحصل على اسم الإجمالي للدالة المحددة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | يضبط قيمة السلسلة المعروضة لقيمة الخلية المنطقية |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | يضبط إعدادات العولمة للمخطط. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | يضبط الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | يضبط اسم الإجمالي الكلي للدالة المحددة. |
| [setListSeparator(char c)](#setListSeparator-char-) | يضبط الفاصل للقائمة، ومعلمات الدالة، ...إلخ. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | يضبط النص المعتمد على الإعدادات المحلية للاسم المدمج بالنص القياسي المعطى. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | يضبط اسم الدالة المعتمد على الإعدادات المحلية المتطابق مع اسم الدالة القياسي المعطى. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | يضبط إعدادات العولمة لجدول المحور. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | يضبط الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | يضبط اسم النوع لصفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | يضبط اسم النوع لصفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | يضبط اسم النوع لصفوف الجدول التي تتكون من رأس الجدول. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | يضبط اسم الإجمالي للدالة المحددة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| v1 | java.lang.String | السلسلة الأولى |
| v2 | java.lang.String | السلسلة الثانية |
| ignoreCase | boolean | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

**Returns:**
int - عدد صحيح يشير إلى العلاقة المعجمية بين المقارنتين
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


يحصل على اسم التسمية "(All)" في PivotTable.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة GlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم التسمية "(All)" label
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


يحصل على قيمة السلسلة المعروضة لقيمة منطقية للخلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| bv | boolean | قيمة منطقية |

**Returns:**
java.lang.String - بشكل افتراضي تُعيد \"TRUE\" للقيمة true و \"FALSE\" للقيمة false.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


يحصل على إعدادات العولمة للمخطط.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


يحوّل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| v | java.lang.String | يجب مقارنة قيمة السلسلة مع القيم الأخرى. |
| ignoreCase | boolean | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

**Returns:**
java.lang.Comparable - يمكن استخدام الكائن للمقارنة أو فرز قيم السلسلة
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


يحصل على اسم التسمية "Column Labels" في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم تسميات الأعمدة
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). نوع عنوان التعليق |

**Returns:**
java.lang.String - اسم عنوان التعليق حسب الإعدادات الإقليمية
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


يحصل على اسم رأس حقل منطقة القيمة في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم رأس حقل البيانات
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


يحصل على اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا. الافتراضي هو \"Sheet\".

**Remarks**

سيكون اسم الورقة التي تُضاف تلقائيًا (مثلًا عبر [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) هو الاسم المحدد متبوعًا برقم تسلسلي. على سبيل المثال، قد يرغب المستخدم الألماني أن يكون اسم الورقة \"Tabellenblatt2\" بدلاً من \"Sheet2\". ثم يمكن للمستخدم تنفيذ هذه الطريقة لإرجاع \"Tabellenblatt\".

**Returns:**
java.lang.String - اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


يحصل على اسم التسمية "(blank)" في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم البيانات الفارغة
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


يحصل على قيمة السلسلة المعروضة لقيمة الخطأ في الخلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| err | java.lang.String | قيم الأخطاء مثل \\#VALUE!,\\#NAME? |

**Returns:**
java.lang.String - بشكل افتراضي تُعيد قيمة الخطأ نفسها
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


يحصل على اسم الإجمالي الكلي للدالة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). نوع الدالة. |

**Returns:**
java.lang.String - اسم الإجمالي الكلي للدالة.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


يحصل على الفاصل للقائمة، ومعلمات الدالة، ...إلخ.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


يحصل على النص المعتمد على الإعدادات الإقليمية للاسم المدمج وفقًا للنص القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | java.lang.String | نص Standard(en-US locale) للاسم المدمج. |

**Returns:**
java.lang.String - نص يعتمد على الإعدادات الإقليمية. تم تحديد الإقليم بواسطة المصنف الذي تُستخدم له هذه الإعدادات.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


يحصل على اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | java.lang.String | اسم الدالة Standard(en-US locale). |

**Returns:**
java.lang.String - اسم الدالة يعتمد على الإعدادات الإقليمية. تم تحديد الإقليم بواسطة المصنف الذي تُستخدم له هذه الإعدادات.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


يحصل على اسم التسمية "(Multiple Items)" في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم التسمية \"(Multiple Items)\"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


يحصل على اسم التسمية "Grand Total" في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم التسمية "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


يحصل على إعدادات العولمة لجدول PivotTable.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


يحصل على اسم التسمية "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم التسمية "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


يحصل على اسم الحماية في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetTextOfProtectedName(string). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم الحماية لـ PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


يحصل على اسم التسمية "Row Labels" في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم تسميات الصفوف
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


يحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على الإعدادات الإقليمية المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | java.lang.String | نص يعتمد على اللغة للاسم المدمج. تم تحديد اللغة بواسطة المصنف (Workbook) الذي تُستخدم له هذه الإعدادات. |

**Returns:**
java.lang.String - نص قياسي (locale en-US).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


يحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعدادات الإقليمية المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | java.lang.String | اسم دالة يعتمد على اللغة. تم تحديد اللغة بواسطة المصنف (Workbook) الذي تُستخدم له هذه الإعدادات. |

**Returns:**
java.lang.String - اسم دالة قياسي (locale en-US).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


يحصل على اسم نمط الخط الإنجليزي القياسي (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط الإقليمي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localfontStyleName | java.lang.String | اسم نمط الخط للغة للعنوان/التذييل. |

**Returns:**
java.lang.String - اسم نمط الخط القياسي للإنجليزية (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


يحصل على اسم نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - اسم نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. القيمة الافتراضية هي "Data"، لذا في الصيغة "\#Data" تمثل منطقة بيانات الجدول.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. القيمة الافتراضية هي "Headers"، لذا في الصيغة "\#Headers" تمثل رأس الجدول.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


يحصل على اسم الإجمالي للدالة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). نوع الدالة. |

**Returns:**
java.lang.String - الاسم الكلي للدالة.
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




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


يضبط قيمة السلسلة المعروضة لقيمة الخلية المنطقية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| bv | boolean | قيمة منطقية |
| name | java.lang.String | قيمة سلسلة للقيمة المنطقية |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


يضبط إعدادات العولمة للمخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


يضبط الفاصل للعناصر في بيانات صف المصفوفة في الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | char | الفاصل المحدد |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). نوع عنوان التعليق |
| name | java.lang.String | اسم عنوان التعليق المعتمد على اللغة |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


يضبط اسم الإجمالي الكلي للدالة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). نوع الدالة. |
| name | java.lang.String | اسم الإجمالي الكلي للدالة. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


يضبط الفاصل للقائمة، ومعلمات الدالة، ...إلخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | char | الفاصل المحدد |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


يضبط النص المعتمد على الإعدادات المحلية للاسم المدمج بالنص القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | java.lang.String | نص اسم المعيار (en-US locale) للاسم المدمج. |
| localName | java.lang.String | نص اسم يعتمد على اللغة. |
| bidirectional | boolean | ما إذا كان سيتم تحويل نص الاسم المحلي إلى نص الاسم المعياري تلقائيًا. إذا كان صحيحًا، سيتم تحويل نص الاسم المحلي إلى نص الاسم المعياري تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) مرة أخرى لنفس زوج الأسماء المعيارية والمحلية |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


يضبط اسم الدالة المعتمد على الإعدادات المحلية المتطابق مع اسم الدالة القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | java.lang.String | اسم الدالة Standard(en-US locale). |
| localName | java.lang.String | اسم الدالة يعتمد على اللغة. |
| bidirectional | boolean | ما إذا كان سيتم تحويل اسم الدالة المحلي إلى اسم الدالة المعياري تلقائيًا. إذا كان صحيحًا، سيتم تحويل الاسم المحلي إلى الاسم المعياري تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) مرة أخرى لنفس زوج الأسماء المعيارية والمحلية |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


يضبط إعدادات العولمة لجدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


يضبط الفاصل للصفوف في بيانات المصفوفة في الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | char | الفاصل المحدد |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | java.lang.String | اسم الدالة يعتمد على اللغة. |
| standardName | java.lang.String | اسم الدالة Standard(en-US locale). |
| bidirectional | boolean | ما إذا كان سيتم تحويل نص الاسم المعياري إلى نص الاسم المحلي تلقائيًا. إذا كان صحيحًا، سيتم تحويل نص الاسم المعياري إلى نص الاسم المحلي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) مرة أخرى لنفس زوج الأسماء المعيارية والمحلية |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | java.lang.String | اسم الدالة يعتمد على اللغة. |
| standardName | java.lang.String | اسم الدالة Standard(en-US locale). |
| bidirectional | boolean | ما إذا كان سيتم تحويل اسم الدالة المعياري إلى اسم الدالة المحلي تلقائيًا. إذا كان صحيحًا، سيتم تحويل الاسم المعياري إلى الاسم المحلي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) مرة أخرى لنفس زوج الأسماء المعيارية والمحلية |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


يضبط اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| localfontStyleName | java.lang.String | اسم نمط الخط للغة للعنوان/التذييل. |
| standardName | java.lang.String | اسم الدالة Standard(en-US locale). |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


يضبط اسم النوع لصفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نوع صفوف الجدول |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نوع صفوف الجدول |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


يضبط اسم النوع لصفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نوع صفوف الجدول |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


يضبط اسم النوع لصفوف الجدول التي تتكون من رأس الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نوع صفوف الجدول |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نوع صفوف الجدول |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


يضبط اسم الإجمالي للدالة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). نوع الدالة. |
| name | java.lang.String | الاسم الكلي للدالة. |

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

