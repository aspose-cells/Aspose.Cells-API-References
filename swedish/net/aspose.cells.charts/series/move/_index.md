---
title: "Series.Move"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-metod. Flyttar serien upp eller ner"
type: docs
url: /sv/net/aspose.cells.charts/series/move/
---
## Series.Move method

Flyttar serien upp eller ner.

```csharp
public void Move(int count)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| antal | Int32 | Antalet steg för att flytta upp eller ner. Flytta serien upp om detta är mindre än noll; flytta serien ner om detta är större än noll. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Hämta den första serien
            Series series = chart.NSeries[0];
            
            try
            {
                // Anropa Move-metoden med Int32-parameter
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Visa effekten genom att ändra seriens namn
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


