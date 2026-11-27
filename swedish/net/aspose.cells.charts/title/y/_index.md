---
title: "Title.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title-egenskapen. Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/title/y/
---
## Title.Y property

Hämtar eller anger y-koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd Title.YRatioToChart‑egenskapen istället. Y = YRatioToChart * 4000; Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange diagramtitel
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Beräkna diagrammet för att säkerställa att layouten uppdateras
            chart.Calculate();

            // Lägg till en form som är justerad med titelns Y‑position
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


