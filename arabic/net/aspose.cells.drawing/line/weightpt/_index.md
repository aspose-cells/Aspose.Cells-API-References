---
title: "Line.WeightPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. يحصل على أو يضبط وزن الخط بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

يحصل على أو يضبط وزن الخط بوحدة النقاط.

```csharp
public double WeightPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPtDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تكوين تسميات البيانات
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.HasLeaderLines = true;

            // تخصيص خطوط القادة
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
            series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
            series.LeaderLines.Color = Color.LightCyan;

            // احفظ المصنف
            workbook.Save("LeaderLinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


