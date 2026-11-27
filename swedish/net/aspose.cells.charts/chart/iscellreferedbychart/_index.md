---
title: "Chart.IsCellReferedByChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-metod. Returnerar om cellen refereras av diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

Returnerar om cellen som diagrammet refererar till.

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Index för bladet -1 betyder kalkylbladet som innehåller det aktuella diagrammet. |
| rowIndex | Int32 | Radindexet |
| columnIndex | Int32 | Kolumnindexet |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
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
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Kontrollera om cellen refereras av diagrammet
            bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
            Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


