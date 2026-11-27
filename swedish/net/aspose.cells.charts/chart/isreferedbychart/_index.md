---
title: "Chart.IsReferedByChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Returnerar om cellen refereras av diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/isreferedbychart/
---
## Chart.IsReferedByChart method

Returnerar om cellen refereras av diagrammet.

```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindexet |
| columnIndex | Int32 | Kolumnindexet |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället metoden IsCellReferedByChart(int,int,int). Denna metod kommer att tas bort 12 månader efter april 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsReferedByChartWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Kontrollera om cell B2 (rad 1, kolumn 1) refereras av diagrammet
                bool isReferred = chart.IsReferedByChart(1, 1);
                
                Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
                
                // Kontrollera en cell som inte finns i diagrammets dataintervall
                bool isNotReferred = chart.IsReferedByChart(10, 10);
                Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


