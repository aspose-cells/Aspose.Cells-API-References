---
title: "Chart.Legend"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑egenskap. Hämtar diagrammets legend"
type: docs
url: /sv/net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Hämtar diagrammets förklaring.

```csharp
public Legend Legend { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyLegendDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Anpassa legend
            chart.Legend.IsAutomaticSize = false;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.Width = 400;
            chart.Legend.Height = 50;
            chart.Legend.Font.Size = 12;
            chart.Legend.Font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("ChartLegendDemo.xlsx");
        }
    }
}
```

### Se även

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


