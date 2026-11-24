---
title: "ChartPointCollection.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPointCollection-Methode. Gibt einen Enumerator für die gesamte ChartPointCollection zurück"
type: docs
url: /de/net/aspose.cells.charts/chartpointcollection/getenumerator/
---
## ChartPointCollection.GetEnumerator method

Gibt einen Enumerator für die gesamte [`ChartPointCollection`](../) zurück.

```csharp
public IEnumerator GetEnumerator()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Holen Sie die Punktesammlung der ersten Serie
                ChartPointCollection points = chart.NSeries[0].Points;

                // Rufen Sie die GetEnumerator-Methode auf
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

            // Ergebnis speichern
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


