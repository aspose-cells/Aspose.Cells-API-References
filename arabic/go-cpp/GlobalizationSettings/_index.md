---
title: "GlobalizationSettings فئة"
linktitle: "GlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "GlobalizationSettings فئة. يحتوي على الكائن الذي يمثل globalizationsettings في Go."
type: docs
weight: 200
url: /ar/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

يمثل إعدادات العولمة.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetChartSettings](./getchartsettings/) | يحصل على إعدادات العولمة لـ Chart. |
| [SetChartSettings](./setchartsettings/) | يضبط إعدادات العولمة لـ Chart. |
| [GetPivotSettings](./getpivotsettings/) | يحصل على إعدادات العولمة لجدول محوري. |
| [SetPivotSettings](./setpivotsettings/) | يضبط إعدادات العولمة لجدول محوري. |
| [GetTotalName](./gettotalname/) | يحصل على الاسم الإجمالي للدالة. |
| [GetGrandTotalName](./getgrandtotalname/) | يحصل على اسم الإجمالي الكلي للدالة. |
| [GetDefaultSheetName](./getdefaultsheetname/) | يحصل على اسم الورقة الافتراضي لإضافة ورقة عمل تلقائيًا. القيمة الافتراضية هي "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. القيمة الافتراضية هي "Headers"، لذا في الصيغة "#Headers" تمثل رأس الجدول. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. القيمة الافتراضية هي "Data"، لذا في الصيغة "#Data" تمثل منطقة البيانات للجدول. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | يحصل على اسم النوع لصفوف الجدول التي تتكون من جميع الصفوف في الجدول المرجعي. القيمة الافتراضية هي "All"، لذا في الصيغة "#All" تمثل جميع الصفوف في الجدول المرجعي. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | يحصل على اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المرجعي. القيمة الافتراضية هي "Totals"، لذا في الصيغة "#Totals" تمثل الصف الإجمالي للجدول المرجعي. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | يحصل على اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المرجعي. القيمة الافتراضية هي "This Row"، لذا في الصيغة "#This Row" تمثل الصف الحالي في الجدول المرجعي. |
| [GetErrorValueString](./geterrorvaluestring/) | يحصل على قيمة السلسلة المعروضة لقيمة الخطأ في الخلية |
| [GetBooleanValueString](./getbooleanvaluestring/) | يحصل على قيمة السلسلة المعروضة لقيمة بوليانية في الخلية |
| [GetLocalFunctionName](./getlocalfunctionname/) | يحصل على اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [GetStandardFunctionName](./getstandardfunctionname/) | يحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعدادات الإقليمية المعطى. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | يحصل على النص المعتمد على الإعدادات الإقليمية للاسم المدمج وفقًا للنص القياسي المعطى. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | يحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على الإعدادات الإقليمية المعطى. |
| [GetListSeparator](./getlistseparator/) | يحصل على الفاصل للقوائم، ومعاملات الدالة، ... إلخ. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | يحصل على اسم نمط الخط الإنجليزي القياسي (Regular, Bold, Italic) للترويسة/التذييل وفقًا لاسم نمط الخط المحلي المعطى. |
| [GetCommentTitleName](./getcommenttitlename/) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| [Compare](./compare/) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. |
