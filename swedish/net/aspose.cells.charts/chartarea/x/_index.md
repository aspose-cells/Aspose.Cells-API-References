---
title: "ChartArea.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea‑egenskap. Hämtar eller anger det horisontella offsetet från dess övre vänstra kolumn i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Hämtar eller anger det horisontella offsetet från dess övre vänstra kolumn, i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ChartArea.XRatioToChart‑egenskapen. X = XRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera diagramområdet
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Spara utdata
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


