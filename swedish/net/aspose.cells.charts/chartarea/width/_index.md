---
title: "ChartArea.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea-egenskap. Hämtar eller anger det horisontella offsetet från dess nedre högra hörnkolumn i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Hämtar eller anger det horisontella offsetet från dess nedre högra hörnkolumn, i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartArea.WidthRatioToChart‑egenskap. Width = WidthRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthDemo
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

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Ange och demonstrera Width‑egenskapen
            Console.WriteLine("Original Width: " + chartArea.Width);
            chartArea.Width = 800; // Set new width
            Console.WriteLine("Modified Width: " + chartArea.Width);

            // Spara arbetsboken
            workbook.Save("ChartAreaWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


