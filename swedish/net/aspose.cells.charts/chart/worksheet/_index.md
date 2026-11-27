---
title: "Chart.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Hämtar kalkylbladet som innehåller detta diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Hämtar kalkylbladet som innehåller detta diagram.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Demonstrera användning av Worksheet-egenskap
            Console.WriteLine("Chart's worksheet index: " + chart.Worksheet.Index);
            Console.WriteLine("Chart's worksheet name: " + chart.Worksheet.Name);
            
            // Spara arbetsboken
            workbook.Save("ChartPropertyWorksheetDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


