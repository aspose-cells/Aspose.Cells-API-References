---
title: "Enum PlotEmptyCellsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Representerar alla tomma celltyper i ett diagram."
type: docs
url: /sv/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Representerar alla tomma celltyper för ett diagram.

```csharp
public enum PlotEmptyCellsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| NotPlotted | `0` | Ej plottad (lämna gap) |
| Zero | `1` | Noll |
| Interpolated | `2` | Interpolerad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:B5", true);

            // Ange diagrammets titel
            chart.Title.Text = "Plot Empty Cells Example";

            // Ställ in hur tomma celler ska plottas
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Spara arbetsboken
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


