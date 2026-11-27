---
title: "ChartFrame.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Anmärkningar

Hur konverterar man enheter av 1/4000 till pixlar? Y i pixlar = Y * Chart.ChartObject.Height / 4000d;

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.YRatioToChart. Y = YRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Åtkomst till diagramrubrik och ange Y‑position
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Spara arbetsboken
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


