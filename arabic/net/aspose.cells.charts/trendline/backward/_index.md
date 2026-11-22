---
title: "Trendline.Backward"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تُرجع أو تُعيّن عدد الفترات أو الوحدات في مخطط مبعثر حيث يمتد خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عمودًا يجب أن يكون عدد الفترات بين 0 و 0.5"
type: docs
url: /ar/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

إرجاع أو تعيين عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد إليها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عمودياً، يجب أن يكون عدد الفترات بين 0 و 0.5

```csharp
public double Backward { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // أضف خط الاتجاه واحصل عليه حسب الفهرس
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // عيّن خاصية backward لتمديد خط الاتجاه إلى الخلف بمقدار 0.5 وحدة
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


