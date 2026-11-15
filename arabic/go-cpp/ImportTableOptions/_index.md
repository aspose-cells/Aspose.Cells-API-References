---
title: "ImportTableOptions Class"
linktitle: "ImportTableOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "ImportTableOptions class. يغلف الكائن الذي يمثل importtableoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/importtableoptions/
---

## ImportTableOptions class

يمثل خيارات استيراد البيانات إلى الخلايا.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | ينشئ خيارات الاستيراد الافتراضية. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetConvertGridStyle](./getconvertgridstyle/) | يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا. |
| [SetConvertGridStyle](./setconvertgridstyle/) | يشير إلى ما إذا كان يتم تطبيق نمط عرض الشبكة على الخلايا. |
| [GetConvertNumericData](./getconvertnumericdata/) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية. |
| [SetConvertNumericData](./setconvertnumericdata/) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحويل قيمة السلسلة إلى قيمة رقمية أو تاريخية. |
| [GetInsertRows](./getinsertrows/) | يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات. |
| [SetInsertRows](./setinsertrows/) | يشير إلى ما إذا كان يجب إضافة صفوف جديدة لاستيراد سجلات البيانات. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | يشير إلى ما إذا كان يتم إزاحة الصف الأول إلى الأسفل عند إدراج الصفوف. |
| [IsFieldNameShown](./isfieldnameshown/) | يشير إلى ما إذا كان يجب استيراد اسم الحقل. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | يشير إلى ما إذا كان يجب استيراد اسم الحقل. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | يشير إلى ما إذا كان يتم تصدير التسمية التوضيحية كاسم حقل |
| [GetDateFormat](./getdateformat/) | يحصل أو يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ/وقت مستوردة. |
| [SetDateFormat](./setdateformat/) | يحصل أو يضبط سلسلة تنسيق التاريخ للخلايا التي تحتوي على قيم تاريخ/وقت مستوردة. |
| [GetNumberFormats](./getnumberformats/) | يحصل أو يضبط تنسيقات الأرقام |
| [SetNumberFormats](./setnumberformats/) | يحصل أو يضبط تنسيقات الأرقام |
| [GetStyles](./getstyles/) | يحصل ويضبط الأنماط لكل عمود في الجدول. |
| [SetStyles](./setstyles/) | يحصل ويضبط الأنماط لكل عمود في الجدول. |
| [GetIsFormulas](./getisformulas/) | يشير إلى ما إذا كانت البيانات صيغًا. |
| [SetIsFormulas](./setisformulas/) | يشير إلى ما إذا كانت البيانات صيغًا. |
| [GetTotalRows](./gettotalrows/) | يحصل أو يضبط إجمالي عدد الصفوف للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [SetTotalRows](./settotalrows/) | يحصل أو يضبط إجمالي عدد الصفوف للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [GetTotalColumns](./gettotalcolumns/) | يحصل أو يضبط إجمالي عدد الأعمدة للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [SetTotalColumns](./settotalcolumns/) | يحصل أو يضبط إجمالي عدد الأعمدة للاستيراد من مصدر البيانات. -1 يعني جميع الصفوف في مصدر البيانات المحدد. |
| [GetColumnIndexes](./getcolumnindexes/) | يحصل أو يضبط الأعمدة (مؤشرها يبدأ من 0) للاستيراد من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة. |
| [SetColumnIndexes](./setcolumnindexes/) | يحصل أو يضبط الأعمدة (مؤشرها يبدأ من 0) للاستيراد من مصدر البيانات. null يعني أنه يجب استيراد جميع الأعمدة. |
| [GetDefaultValues](./getdefaultvalues/) | القيمة الافتراضية للعنصر في الجدول هي null. |
| [SetDefaultValues](./setdefaultvalues/) | القيمة الافتراضية للعنصر في الجدول هي null. |
| [IsHtmlString](./ishtmlstring/) | يشير إلى ما إذا كانت القيمة تحتوي على وسوم html. |
| [SetIsHtmlString](./setishtmlstring/) | يشير إلى ما إذا كانت القيمة تحتوي على وسوم html. |
| [GetCheckMergedCells](./getcheckmergedcells/) | يشير إلى ما إذا كان يتم فحص الخلايا المدمجة. |
| [SetCheckMergedCells](./setcheckmergedcells/) | يشير إلى ما إذا كان يتم فحص الخلايا المدمجة. |
