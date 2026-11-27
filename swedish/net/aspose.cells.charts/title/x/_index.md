---
title: "Title.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title-egenskapen. Hämtar eller anger X-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/title/x/
---
## Title.X property

Hämtar eller anger X-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd Title.XRatioToChart‑egenskapen istället. X = XRatioToChart * 4000; Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Lägg till diagram och ange data
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ange diagramtitelns egenskaper med X‑position
            chart.Title.Text = "Sample Chart";
            chart.Title.X = 200; // Demonstrating X property usage
            chart.Title.Y = 50;

            // Spara arbetsboken
            workbook.Save("TitlePropertyXDemo.xlsx");
        }
    }
}
```

### Se även

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


