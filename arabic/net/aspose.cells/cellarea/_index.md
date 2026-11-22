---
title: "هيكل CellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "هيكل Aspose.Cells.CellArea. يمثل مساحة من الخلايا"
type: docs
url: /ar/net/aspose.cells/cellarea/
---
## CellArea structure

يمثل مساحة من الخلايا.

```csharp
public struct CellArea : IComparable
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | ينشئ مساحة خلية. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | ينشئ مساحة خلية. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | قارن كائنين من CellArea وفقًا للزاوية العلوية اليسرى. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | يرجع سلسلة تمثل كائن مساحة الخلية الحالي. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | يحصل أو يضبط العمود النهائي لهذه المساحة. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | يحصل أو يضبط الصف النهائي لهذه المساحة. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | يحصل أو يضبط العمود الابتدائي لهذه المساحة. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | يحصل أو يضبط الصف الابتدائي لهذه المساحة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // إنشاء مساحة خلية
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // إضافة قاعدة تنسيق شرطي إلى ورقة العمل
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // احفظ المصنف
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // عرض طريقة ToString
            Console.WriteLine(ca.ToString());

            // عرض طريقة CompareTo
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


