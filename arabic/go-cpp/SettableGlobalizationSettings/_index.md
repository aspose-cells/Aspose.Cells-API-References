---
title: "فئة SettableGlobalizationSettings"
linktitle: "SettableGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة SettableGlobalizationSettings. يغلف الكائن الذي يمثل settableglobalizationsettings في Go."
type: docs
weight: 200
url: /ar/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

تنفيذ GlobalizationSettings الذي يدعم المستخدم في تعيين/تغيير النصوص المعرفة مسبقًا.

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetTotalName](./gettotalname/) | يحصل على الاسم الكامل للدالة المحددة. |
| [SetTotalName](./settotalname/) | يضبط الاسم الكامل للدالة المحددة. |
| [GetGrandTotalName](./getgrandtotalname/) | يحصل على اسم الإجمالي الكلي للدالة. |
| [SetGrandTotalName](./setgrandtotalname/) | يضبط اسم الإجمالي الكلي للدالة المحددة. |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. القيمة الافتراضية هي "Headers"، لذا في الصيغة "#Headers" تمثل رأس الجدول. |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | يضبط اسم نوع صفوف الجدول التي تتكون من رأس الجدول. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. القيمة الافتراضية هي "Data"، لذا في الصيغة "#Data" تمثل منطقة البيانات للجدول. |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | يضبط اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | يضبط اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | يضبط اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | يضبط اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| [GetErrorValueString](./geterrorvaluestring/) | يحصل على قيمة السلسلة المعروضة لقيمة الخطأ في الخلية |
| [GetBooleanValueString](./getbooleanvaluestring/) | يحصل على قيمة السلسلة المعروضة لقيمة بوليانية في الخلية |
| [SetBooleanValueString](./setbooleanvaluestring/) | يضبط قيمة السلسلة المعروضة لقيمة بوليانية في الخلية |
| [GetLocalFunctionName](./getlocalfunctionname/) | يحصل على اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [SetLocalFunctionName](./setlocalfunctionname/) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية المقابل لاسم الدالة القياسي المعطى. |
| [GetStandardFunctionName](./getstandardfunctionname/) | يحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعدادات الإقليمية المعطى. |
| [SetStandardFunctionName](./setstandardfunctionname/) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | يحصل على النص المعتمد على الإعدادات الإقليمية للاسم المدمج وفقًا للنص القياسي المعطى. |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | يضبط النص المعتمد على الإعدادات الإقليمية للاسم المدمج بالنص القياسي للاسم المعطى. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | يحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على الإعدادات الإقليمية المعطى. |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [GetListSeparator](./getlistseparator/) | يحصل على الفاصل للقوائم، ومعاملات الدالة، ... إلخ. |
| [SetListSeparator](./setlistseparator/) | يضبط الفاصل للقوائم، ومعاملات الدالة، ... إلخ. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | يضبط الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | يضبط الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | يحصل على اسم نمط الخط الإنجليزي القياسي (Regular, Bold, Italic) للترويسة/التذييل وفقًا لاسم نمط الخط المحلي المعطى. |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [GetCommentTitleName](./getcommenttitlename/) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| [SetCommentTitleName](./setcommenttitlename/) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
