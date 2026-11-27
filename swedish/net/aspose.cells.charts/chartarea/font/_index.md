---
title: "ChartArea.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea-egenskap. Hämtar ett Font‑objekt för det angivna ChartArea‑objektet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

Hämtar ett `Font`‑objekt för det angivna ChartArea‑objektet.

```csharp
public override Font Font { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(4000);
            worksheet.Cells["B5"].PutValue(6000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Hämta diagramområdet
            ChartArea chartArea = chart.ChartArea;
            
            // Ställ in teckensnittsegenskaper för diagramområde
            Aspose.Cells.Font font = chartArea.Font;
            font.Name = "Tahoma";
            font.Size = 10;
            font.Color = Color.Blue;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Spara arbetsboken
            workbook.Save("ChartAreaFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


