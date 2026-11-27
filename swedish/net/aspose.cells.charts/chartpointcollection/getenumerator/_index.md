---
title: "ChartPointCollection.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPointCollection-metod. Returnerar en enumerator för hela ChartPointCollection"
type: docs
url: /sv/net/aspose.cells.charts/chartpointcollection/getenumerator/
---
## ChartPointCollection.GetEnumerator method

Returnerar en enumerator för hela [`ChartPointCollection`](../).

```csharp
public IEnumerator GetEnumerator()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class ChartPointCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
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

            try
            {
                // Hämta den första seriens punktkollektion
                ChartPointCollection points = chart.NSeries[0].Points;

                // Anropa GetEnumerator-metoden
                IEnumerator enumerator = points.GetEnumerator();

                Console.WriteLine("Iterating through chart points:");
                while (enumerator.MoveNext())
                {
                    ChartPoint point = (ChartPoint)enumerator.Current;
                    Console.WriteLine($"Point value: {point.YValue}");
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


