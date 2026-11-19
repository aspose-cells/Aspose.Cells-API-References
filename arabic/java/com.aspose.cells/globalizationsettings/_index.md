---
title: "GlobalizationSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعدادات العولمة."
type: docs
url: /ar/java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

يمثل إعدادات العولمة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
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
| [getTotalName(int functionType)](#getTotalName-int-) | يحصل على الاسم الكلي للدالة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | يضبط إعدادات العولمة للمخطط. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | يضبط إعدادات العولمة لجدول المحور. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
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
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). |

**Returns:**
java.lang.String -
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


يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. القيمة الافتراضية هي "All"، لذا في الصيغة "\#All" تمثل جميع الصفوف في الجدول المشار إليه.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. القيمة الافتراضية هي "This Row"، لذا في الصيغة "\#This Row" تمثل الصف الحالي في الجدول المشار إليه.

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


يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. القيمة الافتراضية هي "Totals"، لذا في الصيغة "\#Totals" تمثل الصف الإجمالي للجدول المشار إليه.

**Returns:**
java.lang.String - اسم نوع صفوف الجدول
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


يحصل على الاسم الكلي للدالة.

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




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


يضبط إعدادات العولمة للمخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


يضبط إعدادات العولمة لجدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

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

