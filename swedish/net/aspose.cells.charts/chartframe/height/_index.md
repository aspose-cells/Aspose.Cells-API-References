---
title: "ChartFrame.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar eller anger höjden på ramen i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Hämtar eller anger höjden på ramen i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Anmärkningar

Hur konverterar man enheter av 1/4000 till pixlar? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

OBS: Denna medlem är nu föråldrad. Använd ChartFrame.HeightRatioToChart‑egenskapen istället. Height = HeightRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
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
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till datamärkningar
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Ställ in Height‑egenskapen
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Visa höjdvärdet
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Spara arbetsboken
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


