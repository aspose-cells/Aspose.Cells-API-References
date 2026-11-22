---
title: "TickLabels.IsAutomaticRotation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تشير إلى ما إذا كانت زاوية الدوران تلقائية"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/isautomaticrotation/
---
## TickLabels.IsAutomaticRotation property

يشير إلى ما إذا كان زاوية الدوران تلقائية

```csharp
public bool IsAutomaticRotation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyIsAutomaticRotationDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تكوين تسميات العلامات
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.IsAutomaticRotation = false; // Disable automatic rotation
            tickLabels.RotationAngle = 45; // Set manual rotation angle

            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


