---
title: "فئة GlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GlobalizationSettings. تمثل إعدادات العولمة"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

يمثل إعدادات العولمة.

```csharp
public class GlobalizationSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | يحصل أو يحدد إعدادات العولمة للمخطط. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | يحصل على الفاصل للقائمة، معلمات الدالة، ...إلخ. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | يحصل أو يحدد إعدادات العولمة لجدول المحور. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) يحصل على اسم التسمية "(All)" في جدول المحور. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | يحصل على قيمة النص المعروض لقيمة الخلية المنطقية |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | يحوّل النص إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) يحصل على اسم التسمية "Column Labels" في جدول المحور. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | يحصل على اسم عنوان التعليق المعتمد على اللغة وفقًا لنوع عنوان التعليق. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) يحصل على اسم رأس حقل منطقة القيم في جدول Pivot. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | يحصل على اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا. الافتراضي هو "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) يحصل على اسم التسمية "(blank)" في جدول Pivot. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | يحصل على قيمة النص المعروض لقيمة خطأ الخلية |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | يحصل على اسم الإجمالي الكلي للدالة. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | يحصل على النص المعتمد على اللغة للاسم المدمج وفقًا للنص المعياري المعطى. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | يحصل على اسم الدالة المعتمد على اللغة وفقًا لاسم الدالة المعياري المعطى. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) يحصل على اسم التسمية "(Multiple Items)" في جدول Pivot. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) يحصل على اسم التسمية "Grand Total" في جدول Pivot. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) يحصل على اسم التسمية "Total" في جدول Pivot. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي جدول Pivot على حقلين Pivot أو أكثر في منطقة البيانات. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) يحصل على اسم الحماية في جدول Pivot. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) يحصل على اسم التسمية "Row Labels" في جدول Pivot. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | يحصل على النص المعياري للاسم المدمج وفقًا للنص المعتمد على اللغة المعطى. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | يحصل على اسم الدالة المعياري وفقًا لاسم الدالة المعتمد على اللغة المعطى. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | يحصل على اسم نمط الخط الإنجليزي المعياري (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط المعتمد على اللغة المعطى. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) يحصل على اسم النوع [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) في جدول Pivot. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من جميع الصفوف في الجدول المشار إليه. الافتراضي هو "All"، لذا في الصيغة "#All" تمثل جميع الصفوف في الجدول المشار إليه. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. الافتراضي هو "This Row"، لذا في الصيغة "#This Row" تمثل الصف الحالي في الجدول المشار إليه. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه. الافتراضي هو "Data"، لذا في الصيغة "#Data" تمثل منطقة البيانات للجدول. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. الافتراضي هو "Headers"، لذا في الصيغة "#Headers" تمثل رأس الجدول. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الإجمالي للجدول المشار إليه. الافتراضي هو "Totals"، لذا في الصيغة "#Totals" تمثل الصف الإجمالي للجدول المشار إليه. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | يحصل على الاسم الإجمالي للدالة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // إنشاء وتطبيق إعدادات العولمة
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // تطبيق المجموع الفرعي مع عولمة مخصصة
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // تخصيص الاسم الإجمالي بناءً على نوع الدالة
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


