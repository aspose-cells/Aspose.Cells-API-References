---
title: "WorksheetCollection فئة"
linktitle: "WorksheetCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "WorksheetCollection فئة. يغلف الكائن الذي يمثل worksheetcollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/worksheetcollection/
---

## WorksheetCollection class

يحتوي على مجموعة من كائنات <see cref=\"Worksheet\"/>.

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | يحصل على قائمة ألواح المهام. |
| [GetWebExtensions](./getwebextensions/) | يحصل على قائمة ألواح المهام. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | يحصل على قائمة مؤلفي التعليقات المتسلسلة. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel. |
| [CreateRange](./createrange/) | ينشئ كائن Range من عنوان النطاق. |
| [CreateUnionRange](./createunionrange/) | ينشئ كائن Range من عنوان النطاق. |
| [GetNames](./getnames/) | يحصل على مجموعة جميع كائنات Name في جدول البيانات. |
| [Get_Int](./get_int/) | يحصل على عنصر Worksheet عند الفهرس المحدد. |
| [Get_String](./get_string/) | يحصل على عنصر Worksheet بالاسم المحدد. |
| [GetSheetByCodeName](./getsheetbycodename/) | يحصل على ورقة العمل بالاسم الرمزي. |
| [GetActiveSheetName](./getactivesheetname/) | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [SetActiveSheetName](./setactivesheetname/) | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [GetActiveSheetIndex](./getactivesheetindex/) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [SetActiveSheetIndex](./setactivesheetindex/) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [SortNames](./sortnames/) | يقوم بترتيب الأسماء المعرفة. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | إدراج ورقة عمل. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | إدراج ورقة عمل. |
| [Add_SheetType](./add_sheettype/) | يضيف ورقة عمل إلى المجموعة. |
| [SwapSheet](./swapsheet/) | يبدل الورقتين. |
| [Add](./add/) | يضيف ورقة عمل إلى المجموعة. |
| [Add_String](./add_string/) | يضيف ورقة عمل إلى المجموعة. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | يضيف وظيفة الإضافة إلى دفتر العمل |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | يضيف وظيفة الإضافة إلى دفتر العمل |
| [RemoveAt_String](./removeat_string/) | يزيل العنصر بالاسم المحدد. |
| [RemoveAt_Int](./removeat_int/) | يزيل العنصر بالفهرس المحدد. |
| [Clear](./clear/) | مسح جميع أوراق العمل. |
| [AddCopy_String](./addcopy_string/) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy_Int](./addcopy_int/) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | نسخ مجموعة من أوراق العمل. |
| [GetDxfs](./getdxfs/) | يحصل على سجلات التنسيق التفاضلي الرئيسية. |
| [GetRangeByName_String](./getrangebyname_string/) | يحصل على كائن Range حسب الاسم المحدد مسبقًا. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | يحصل على Range حسب الاسم المحدد مسبقًا أو اسم الجدول |
| [GetNamedRanges](./getnamedranges/) | يحصل على جميع النطاقات المسماة المحددة مسبقًا في جدول البيانات. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | يحصل على جميع النطاقات المسماة المحددة مسبقًا في جدول البيانات. |
| [GetXmlMaps](./getxmlmaps/) | يحصل على ويضبط خرائط XML في دفتر العمل. |
| [SetXmlMaps](./setxmlmaps/) | يحصل على ويضبط خرائط XML في دفتر العمل. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | يعيد مجموعة DocumentProperty تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | يعيد مجموعة DocumentProperty تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [GetOleSize](./getolesize/) | يحصل على ويضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [SetOleSize_Object](./setolesize_object/) | يحصل على ويضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | يضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole. |
| [GetExternalLinks](./getexternallinks/) | يمثل الروابط الخارجية في دفتر العمل. |
| [GetPivotCaches](./getpivotcaches/) | يحصل على جميع PivotCache. |
| [GetTableStyles](./gettablestyles/) | يحصل على كائن TableStyles. |
| [ClearPivottables](./clearpivottables/) | يمسح جداول Pivot من جدول البيانات. |
| [GetRevisionLogs](./getrevisionlogs/) | يمثل سجلات المراجعة. |
| [RefreshPivotTables](./refreshpivottables/) | يقوم بتحديث جميع PivotTables في ملف Excel. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | يقوم بتحديث جميع PivotTables في ملف Excel. |
| [GetSensitivityLabels](./getsensitivitylabels/) | يمثل جميع تصنيفات الحساسية. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
