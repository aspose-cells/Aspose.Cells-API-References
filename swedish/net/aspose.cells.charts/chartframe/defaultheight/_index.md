---
title: "ChartFrame.DefaultHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultheight/
---
## ChartFrame.DefaultHeight property

Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightDemo
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

            // Åtkomst till diagrammets titel (som är en ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Visa det aktuella DefaultHeight‑värdet (skrivskyddad egenskap)
            Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);

            // Demonstrera hur DefaultHeight påverkar diagrammets layout
            Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
            Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Justera höjden med den skrivbara egenskapen
            chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
            Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Spara resultatet
            workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


