---
title: "ChartPointCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPointCollection-metod. Tar bort punkt vid indexet för serien"
type: docs
url: /sv/net/aspose.cells.charts/chartpointcollection/removeat/
---
## ChartPointCollection.RemoveAt method

Tar bort punkt vid indexet i serien.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Punktens index. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första seriens punktkollektion
            ChartPointCollection points = chart.NSeries[0].Points;

            try
            {
                // Visa initialt antal
                Console.WriteLine($"Initial points count: {points.Count}");

                // Ta bort punkten vid index 1 (andra punkten)
                points.RemoveAt(1);

                // Visa resultatet
                Console.WriteLine($"Points count after RemoveAt: {points.Count}");
                Console.WriteLine("Point at index 1 removed successfully.");

                // Spara arbetsboken
                workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


