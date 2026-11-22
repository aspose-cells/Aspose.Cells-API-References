---
title: "Series.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. يحصل أو يضبط نوع سلسلة البيانات"
type: docs
url: /ar/net/aspose.cells.charts/series/type/
---
## Series.Type property

يحصل على أو يضبط نوع سلسلة البيانات.

```csharp
public ChartType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط عمودي مكدس
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تحقق واطبع نوع السلسلة
            foreach (Series series in chart.NSeries)
            {
                Console.WriteLine("Series Type: " + series.Type);
            }
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


