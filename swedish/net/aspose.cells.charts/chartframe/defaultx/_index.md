---
title: "ChartFrame.DefaultX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Representerar x för standardposition i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Representerar x för standardposition i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd ChartFrame.DefaultXRatioToChart‑egenskapen istället. DefaultX = (int)(DefaultXRatioToChart * 4000); Denna egenskap kommer att tas bort 12 månader senare, sedan februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            
            // Åtkomst till diagramtitel som ärver från ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Visa standard‑X‑positionen för diagramtiteln
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Demonstrera hur standardpositionen påverkar diagrammet
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // Ändra titelns position med hjälp av förhållandeegenskaper (eftersom DefaultX är skrivskyddad)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Spara arbetsboken
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


