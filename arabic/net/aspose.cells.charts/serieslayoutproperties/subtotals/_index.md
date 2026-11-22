---
title: "SeriesLayoutProperties.Subtotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تمثل فهرس نقطة بيانات المجموع الفرعي"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/subtotals/
---
## SeriesLayoutProperties.Subtotals property

يمثل فهرس نقطة بيانات المجموع الفرعي.

```csharp
public int[] Subtotals { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertySubtotalsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين المجموعات الفرعية للسلسلة الأولى
            chart.NSeries[0].LayoutProperties.Subtotals = new int[] { 0, 3 };

            // تحقق من أن المجموعات الفرعية تم تعيينها بشكل صحيح
            Console.WriteLine("Subtotal at index 0: " + chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Console.WriteLine("Subtotal at index 1: " + chart.NSeries[0].LayoutProperties.Subtotals[1]);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


