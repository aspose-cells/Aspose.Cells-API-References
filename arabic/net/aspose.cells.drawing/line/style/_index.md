---
title: "Line.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تمثل نمط الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/style/
---
## Line.Style property

يمثل نمط الخط.

```csharp
public LineType Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء مخطط تجريبي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // احصل على السلسلة الأولى والنقطة الأولى لها
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // حدد خصائص الخط
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // تحقق من ضبط النمط
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


