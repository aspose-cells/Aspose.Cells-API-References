---
title: "TickLabels.BackgroundMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تحصل وتعيّن وضع العرض للخلفية"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/backgroundmode/
---
## TickLabels.BackgroundMode property

يحصل ويضبط وضع عرض الخلفية.

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تكوين تسميات العلامات
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;

            workbook.Save("TickLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BackgroundMode](../../backgroundmode/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


