---
title: "LegendEntry.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LegendEntry. يحصل على كائن Font للعنصر ChartFrame المحدد"
type: docs
url: /ar/net/aspose.cells.charts/legendentry/font/
---
## LegendEntry.Font property

يحصل على كائن `Font` للعنصر ChartFrame المحدد.

```csharp
public Font Font { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            Aspose.Cells.Charts.LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            Aspose.Cells.Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            workbook.Save("LegendEntryFontExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


