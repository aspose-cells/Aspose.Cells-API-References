---
title: "فئة PivotFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Pivot.PivotFilter. تمثّل PivotFilter في مجموعة PivotFilter"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

يمثل PivotFilter في مجموعة PivotFilter.

```csharp
public class PivotFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) يحصل على الفلتر التلقائي لمرشح المحور. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | يحصل على ترتيب التقييم لمرشح المحور. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | يحصل على فهرس حقل المصدر الذي يُطبق عليه هذا مرشح المحور. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | يحصل على فئة هذا المرشح. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | يحصل على نوع المرشح لمرشح المحور. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | يحدد فهرس حقل مكعب القياس. تُستخدم هذه الخاصية فقط بواسطة المرشحات في جداول المحور OLAP وتحدد على أي قياس يجب أن يُطبق مرشح القيمة. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) يحصل على فهرس حقل القياس لمرشح المحور. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | يحصل على فهرس حقل خاصية العضو لمرشح المحور. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | يحصل على اسم مرشح المحور. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | يشير إلى ما إذا كان يجب استخدام أيام كاملة في معايير تصفية التاريخ. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | يحصل على القيمة النصية 1 للملصق في مرشح المحور. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | يحصل على القيمة النصية 2 للملصق في مرشح المحور. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | يحصل على فهرس حقل القيمة في منطقة القيمة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | يحصل على قيم مرشح الأعداد. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | يحصل على تسميات مرشح التسمية. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | يحصل على قيم مرشح الأعداد. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | يحصل على إعداد أعلى 10 للمرشح. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء ورقة العمل ببيانات عينة
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // أضف جدولًا محوريًا إلى ورقة العمل
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // تعيين نمط جدول pivot
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // إضافة مرشح محوري
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // تعيين خصائص إضافية لمرشح المحور
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // تحديث وحساب بيانات جدول المحور
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ المصنف
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


