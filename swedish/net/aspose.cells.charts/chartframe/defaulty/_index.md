---
title: "ChartFrame.DefaultY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Representerar y‑värdet för standardpositionen i enheter av 1/4000 av diagramområdet."
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Representerar y‑värdet för standardpositionen i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart * 4000); Denna egenskap kommer att tas bort 12 månader senare från February 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Åtkomst till diagramtitel som ärver från ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Visa det aktuella DefaultY‑värdet (skrivskyddad egenskap)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Visa hur DefaultY påverkar positionering genom att jämföra med aktuell position
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Återställ position till standard med SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Spara resultatet
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


