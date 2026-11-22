---
title: "Series.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. صحيحة إذا كانت السلسلة لها ظل"
type: docs
url: /ar/net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

صحيح إذا كانت السلسلة تحتوي على ظل.

```csharp
public bool Shadow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى السلسلة الأولى وتمكين الظل
            Series series = chart.NSeries[0];
            series.Shadow = true;

            // احفظ وأعد التحميل للتحقق
            workbook.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Series loadedSeries = loadedWorkbook.Worksheets[0].Charts[0].NSeries[0];
            Console.WriteLine("Shadow enabled: " + loadedSeries.Shadow);
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


