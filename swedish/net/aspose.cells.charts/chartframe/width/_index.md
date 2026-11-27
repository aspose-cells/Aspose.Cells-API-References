---
title: "ChartFrame.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame property. Hämtar eller anger bredden på ramen i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Hämtar eller anger bredden på ramen i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Anmärkningar

Hur konverterar man enheter av 1/4000 till pixlar? Bredd i pixlar = Bredd * Chart.ChartObject.Height / 4000d;

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.WidthRatioToChart. Width = WidthRatioToChart * 4000; Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
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

            // Lägg till ett diagram och hämta dess diagramram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Ställ in och visa den ursprungliga bredden
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Ändra bredden
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Spara arbetsboken
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


