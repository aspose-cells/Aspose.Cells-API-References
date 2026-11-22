---
title: "Trendline.Forward"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تُرجع أو تُعيّن عدد الفترات أو الوحدات في مخطط مبعثر حيث يمتد خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر"
type: docs
url: /ar/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

إرجاع أو تعيين عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد إليها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر.

```csharp
public double Forward { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // إضافة خط اتجاه
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // عرض خاصية Forward
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


