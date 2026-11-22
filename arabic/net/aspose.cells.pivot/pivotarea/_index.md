---
title: "فئة PivotArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotArea فئة. يعرض المنطقة المحددة لجدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

يعرض المنطقة المحددة من جدول Pivot.

```csharp
public class PivotArea
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | يعرض المنطقة المحددة ل PivotTable. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | يحصل ويضبط منطقة PivotTable التي ينطبق عليها هذا القاعدة. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | يحصل على جميع الفلاتر لهذا PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | يشير إلى ما إذا كان المجموع الكلي للعمود مشمولًا. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط التفصيلي. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | يشير إلى ما إذا كان إجمالي الصف الإجمالي مشمولًا. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | يشير إلى ما إذا كانت قيم البيانات فقط (في منطقة البيانات في العرض) لتحديد عنصر ما مختارة ولا تشمل تسميات العنصر. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر ما مختارة. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | يحصل على نوع قاعدة الاختيار ويضبطه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | يحصل على مناطق الخلايا في هذه المنطقة المحورية. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | حدد المنطقة باستخدام المرشحات. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | حدد حقلًا في المنطقة كمنطقة. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | حدد حقلًا في المنطقة كمنطقة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // إنشاء كائن PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);

            // ضبط خصائص PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // استخدم طريقة Select لتحديد منطقة معينة
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // احفظ المصنف
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


