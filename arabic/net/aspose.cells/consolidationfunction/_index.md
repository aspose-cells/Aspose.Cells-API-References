---
title: "تعداد ConsolidationFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ConsolidationFunction enum. يمثل وظيفة التجميع"
type: docs
url: /ar/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

يمثل دالة التجميع.

```csharp
public enum ConsolidationFunction
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Sum | `0` | يمثل دالة Sum. |
| Count | `1` | يمثل دالة Count. |
| Average | `2` | يمثل دالة Average. |
| Max | `3` | يمثل دالة Max. |
| Min | `4` | يمثل دالة Min. |
| Product | `5` | يمثل دالة Product. |
| CountNums | `6` | يمثل دالة Count Nums. |
| StdDev | `7` | يمثل دالة StdDev. |
| StdDevp | `8` | يمثل دالة StdDevp. |
| Var | `9` | يمثل دالة Var. |
| Varp | `10` | يمثل دالة Varp. |
| DistinctCount | `11` | يمثل دالة Distinct Count. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // حدد منطقة الخلية للمجموع الفرعي
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // طبق المجموع الفرعي باستخدام دالة Sum
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // طبق المجموع الفرعي باستخدام دالة Average
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // طبق المجموع الفرعي باستخدام دالة Max
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // طبق المجموع الفرعي باستخدام دالة Min
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // احفظ المصنف
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // أخرج النتائج
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


