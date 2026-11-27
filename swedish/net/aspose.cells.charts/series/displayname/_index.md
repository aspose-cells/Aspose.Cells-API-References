---
title: "Series.DisplayName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Hämtar seriens namn som visas på diagramgrafen"
type: docs
url: /sv/net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Hämtar seriens namn som visas i diagramgrafen.

```csharp
public string DisplayName { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesPropertyDisplayNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Kom åt den första serien och visa dess DisplayName
                Series series = chart.NSeries[0];
                Console.WriteLine("Series DisplayName: " + series.DisplayName);

                // Visa även Name‑egenskapen för jämförelse
                Console.WriteLine("Series Name: " + series.Name);

                // Spara arbetsboken
                workbook.Save("DisplayNameDemo.xlsx");
                Console.WriteLine("DisplayName has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


