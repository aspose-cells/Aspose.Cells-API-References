---
title: "ChartArea.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea‑egenskap. Hämtar eller får det vertikala offsetet från dess övre vänstra rad i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/y/
---
## ChartArea.Y property

Hämtar eller får det vertikala offsetet från dess övre vänstra rad, i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ChartArea.YRatioToChart‑egenskapen. Y = YRatioToChart * 4000; Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera diagramområdet med Y‑egenskapen
            ChartArea chartArea = chart.ChartArea;
            chartArea.Y = 20; // Setting Y position
            chartArea.Height = 250;

            workbook.Save("ChartAreaYExample.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


