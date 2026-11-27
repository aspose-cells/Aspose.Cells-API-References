---
title: "Chart.Move"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart metod. Flyttar diagrammet till en angiven plats"
type: docs
url: /sv/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Flyttar diagrammet till en angiven plats.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| topRow | Int32 | Övre vänstra radindex. |
| rightColumn | Int32 | Index för nedre högra kolumnen |
| bottomRow | Int32 | Index för nedre högra rad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Original diagramposition
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Flytta diagrammet till ny position (rader 10-20, kolumner 2-8)
                chart.Move(10, 2, 20, 8);

                // Visa ny position
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Spara arbetsboken
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


