---
title: "AxisBins.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AxisBins. يحصل على أو يضبط عرض صندوق المحور"
type: docs
url: /ar/net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

يحصل أو يعيّن عرض حاوية المحور.

```csharp
public double Width { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);

            // إنشاء مخطط هيستوجرام
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.CategoryData = "B1:D1";

            // تعيين عرض الصندوق
            chart.CategoryAxis.Bins.Width = 12;

            // حفظ وإظهار النتيجة
            workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");

            Console.WriteLine("Example executed successfully with bin width set to 12.");
        }
    }
}
```

### انظر أيضًا

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


