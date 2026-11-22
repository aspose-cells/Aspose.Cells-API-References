---
title: "فئة SettableGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.SettableGlobalizationSettings. تنفيذ GlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المعرفة مسبقًا"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

تنفيذ GlobalizationSettings الذي يدعم المستخدم في تعيين/تغيير النصوص المحددة مسبقًا.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | يحصل أو يعيّن إعدادات العولمة للمخطط. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | يحصل على الفاصل للقائمة، معلمات الدالة، ...إلخ. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | يحصل أو يعيّن إعدادات العولمة لجدول المحور. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) يحصل على اسم التسمية "(All)" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | يحصل على قيمة النص المعروض لقيمة الخلية المنطقية |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | يحوّل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد الترتيب المحددة. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) يحصل على اسم التسمية "Column Labels" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) يحصل على اسم رأس حقل منطقة القيم في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | يحصل على اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا. الافتراضي هو "Sheet". (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) يحصل على اسم التسمية "(blank)" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | يحصل على قيمة النص المعروض لقيمة خطأ الخلية |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | يحصل على اسم الإجمالي الكلي للدالة. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | يحصل على النص المعتمد على اللغة للاسم المدمج وفقًا للنص المعياري المعطى. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | يحصل على اسم الدالة المعتمد على اللغة وفقًا لاسم الدالة المعياري المعطى. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) يحصل على اسم التسمية "(Multiple Items)" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) يحصل على اسم التسمية "Grand Total" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) يحصل على اسم التسمية "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) يحصل على اسم الحماية في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) يحصل على اسم التسمية "Row Labels" في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | يحصل على النص المعياري للاسم المدمج وفقًا للنص المعتمد على اللغة المعطى. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | يحصل على اسم الدالة المعياري وفقًا لاسم الدالة المعتمد على اللغة المعطى. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | يحصل على اسم نمط الخط الإنجليزي المعياري (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط المعتمد على اللغة المعطى. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) يحصل على اسم النوع [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) في PivotTable. (موروث من [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه. الافتراضي هو "Data"، لذا في الصيغة "#Data" تمثل منطقة البيانات للجدول. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. الافتراضي هو "Headers"، لذا في الصيغة "#Headers" تمثل رأس الجدول. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | يحصل على اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | يحصل على الاسم الكلي للدالة المحددة. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | يضبط قيمة سلسلة العرض لقيمة البوليان للخلية |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | يضبط الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | يضبط اسم الإجمالي الكلي للدالة المحددة. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | يضبط الفاصل للقائمة، ومعلمات الدالة، ...إلخ. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | يضبط النص المعتمد على الإعدادات الإقليمية للاسم المدمج بالنص القياسي المعطى. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية المتوافق مع اسم الدالة القياسي المعطى. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | يضبط الفاصل للصفوف في بيانات المصفوفة في الصيغة. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | يضبط اسم النوع لصفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | يضبط اسم النوع لصفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | يضبط اسم النوع لصفوف الجدول التي تتكون من رأس الجدول. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | يضبط اسم النوع لصفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | يضبط الاسم الكلي للدالة المحددة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // ضبط فاصل قائمة مخصص
            settings.SetListSeparator(';');

            // ضبط سلاسل قيم بوليان مخصصة
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // ضبط أسماء دوال مخصصة
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // ضبط أسماء أنواع صفوف جدول مخصصة
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // ضبط أسماء عناوين تعليقات مخصصة
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // تم إزالة سطر المؤلف لأن CommentTitleType لا يحتوي على قيمة التعداد تلك
            // إذا كنت بحاجة إلى ضبط إعدادات متعلقة بالمؤلف، فستحتاج إلى استخدام ThreadedCommentAuthor بدلاً من ذلك

            // تطبيق إعدادات العولمة على دفتر العمل
            workbook.Settings.GlobalizationSettings = settings;

            // إظهار الاستخدام في الصيغ
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // احفظ المصنف
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


