---
title: "ChartFrame.DefaultWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Åtkomst till diagramrubriken (som ärver från ChartFrame)
            Title title = chart.Title;
            
            // Visa standardbredden för diagramramen (rubrik i detta fall)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Obs: DefaultWidth är skrivskyddad, så vi kan inte sätta den
            // Vi kan bara läsa den för att förstå standarddimensionerna
            
            // Demonstrera hur denna egenskap påverkar diagrammet
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Spara arbetsboken
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


