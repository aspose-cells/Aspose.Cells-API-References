---
title: "فئة ListObject"
linktitle: "ListObject"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ListObject. يحتوي على الكائن الذي يمثل listobject في Go."
type: docs
weight: 200
url: /ar/go-cpp/listobject/
---

## ListObject class

يمثل جدولًا في ورقة عمل.

```go

type ListObject struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetStartRow](./getstartrow/) | يحصل على صف البداية للنطاق. |
| [GetStartColumn](./getstartcolumn/) | يحصل على عمود البداية للنطاق. |
| [GetEndRow](./getendrow/) | يحصل على صف النهاية للنطاق. |
| [GetEndColumn](./getendcolumn/) | يحصل على عمود النهاية للنطاق. |
| [GetListColumns](./getlistcolumns/) | يحصل على قائمة ListColumn لهذا الجدول. |
| [Resize](./resize/) | تغيير حجم النطاق لكائن القائمة. |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | ضع القيمة في الخلية. |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | ضع القيمة في الخلية. |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | ضع الصيغة في الخلية داخل الجدول. |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | ضع الصيغة في الخلية داخل الجدول. |
| [GetShowHeaderRow](./getshowheaderrow/) | يحصل ويضبط ما إذا كان هذا الجدول يظهر صف الرأس. |
| [SetShowHeaderRow](./setshowheaderrow/) | يحصل ويضبط ما إذا كان هذا الجدول يظهر صف الرأس. |
| [GetShowTotals](./getshowtotals/) | يحصل ويضبط ما إذا كان هذا TAble يظهر صف الإجمالي. |
| [SetShowTotals](./setshowtotals/) | يحصل ويضبط ما إذا كان هذا TAble يظهر صف الإجمالي. |
| [GetDataRange](./getdatarange/) | يحصل على نطاق البيانات للجدول. |
| [UpdateColumnName](./updatecolumnname/) | يحدّث أسماء جميع أعمدة القائمة إلى الخلايا في الجدول. |
| [GetQueryTable](./getquerytable/) | يحصل على QueryTable المرتبط. |
| [GetDataSourceType](./getdatasourcetype/) | يحصل على نوع مصدر البيانات للجدول. |
| [GetHasAutoFilter](./gethasautofilter/) | يشير إلى ما إذا كان تم تطبيق الفلتر التلقائي على هذا الجدول. |
| [SetHasAutoFilter](./sethasautofilter/) | يشير إلى ما إذا كان تم تطبيق الفلتر التلقائي على هذا الجدول. |
| [RemoveAutoFilter](./removeautofilter/) | يزيل الفلتر التلقائي المطبق على هذا الجدول. |
| [GetAutoFilter](./getautofilter/) | يحصل على الفلتر التلقائي لهذا الجدول. |
| [GetDisplayName](./getdisplayname/) | يحصل ويضبط اسم العرض للجدول. |
| [SetDisplayName](./setdisplayname/) | يحصل ويضبط اسم العرض للجدول. |
| [GetComment](./getcomment/) | يحصل ويضبط تعليق الجدول. |
| [SetComment](./setcomment/) | يحصل ويضبط تعليق الجدول. |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق عليه. |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق عليه. |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق عليه. |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق عليه. |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | يشير إلى ما إذا كان تنسيق الخطوط المتناوبة للصفوف مطبقًا. |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | يشير إلى ما إذا كان تنسيق الخطوط المتناوبة للصفوف مطبقًا. |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | يشير إلى ما إذا كان تنسيق الخطوط المتناوبة للأعمدة مطبقًا. |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | يشير إلى ما إذا كان تنسيق الخطوط المتناوبة للأعمدة مطبقًا. |
| [ApplyStyleToRange](./applystyletorange/) | طبق نمط الجدول على النطاق. |
| [ConvertToRange](./converttorange/) | حوّل الجدول إلى نطاق. |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | حوّل الجدول إلى نطاق. |
| [GetTableStyleType](./gettablestyletype/) | يحصل على نمط الجدول المدمج. |
| [SetTableStyleType](./settablestyletype/) | يحصل على نمط الجدول المدمج. |
| [GetTableStyleName](./gettablestylename/) | يحصل ويضبط اسم نمط الجدول. |
| [SetTableStyleName](./settablestylename/) | يحصل ويضبط اسم نمط الجدول. |
| [GetXmlMap](./getxmlmap/) | يحصل على XmlMap المستخدم لهذه القائمة. |
| [GetAlternativeText](./getalternativetext/) | يحصل ويضبط النص البديل. |
| [SetAlternativeText](./setalternativetext/) | يحصل ويضبط النص البديل. |
| [GetAlternativeDescription](./getalternativedescription/) | يسترجع ويضبط الوصف البديل. |
| [SetAlternativeDescription](./setalternativedescription/) | يسترجع ويضبط الوصف البديل. |
