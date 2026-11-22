---
title: "DataLabels.Area"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تحصّل على المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/area/
---
## DataLabels.Area property

يحصل على `area`.

```csharp
public override Area Area { get; }
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
    public class DataLabelsPropertyAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // بيانات عينة
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Scatter, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // تكوين منطقة تسميات البيانات
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // عرض استخدام خاصية Area
            series.DataLabels.Area.FillFormat.Pattern = FillPattern.Solid;
            series.DataLabels.Area.BackgroundColor = Color.LightBlue;
            series.DataLabels.Area.ForegroundColor = Color.White;
            series.DataLabels.Area.Transparency = 0.3;
            
            workbook.Save("DataLabelsAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Area](../../../aspose.cells.drawing/area/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


