---
title: "Enum ChartSplitType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartSplitType enum. Representerar hur de två sektionerna i antingen ett paj‑paj‑diagram eller ett stapel‑paj‑diagram delas upp."
type: docs
url: /sv/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Representerar hur de två sektionerna i antingen ett paj‑i‑paj‑diagram eller ett stapel‑i‑paj‑diagram delas upp.

```csharp
public enum ChartSplitType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Position | `0` | Representerar datapunkterna. Datapunkterna ska delas mellan pajen och det andra diagrammet genom att placera den sista delningspositionen för datapunkterna i det andra diagrammet. |
| Value | `1` | Representerar att datapunkterna ska delas mellan pajen och det andra diagrammet genom att placera datapunkterna med värde mindre än delningspositionen i det andra diagrammet. |
| PercentValue | `2` | Representerar datapunkterna som ska delas mellan pajen och det andra diagrammet genom att placera punkterna med en procentandel mindre än delningspositionen i procent i det andra diagrammet. |
| Custom | `3` | Representerar att datapunkterna ska delas mellan pajen och det andra diagrammet enligt de anpassade delningsvärdena. |
| Auto | `4` | Representerar datapunkterna som ska delas med standardmekanismen för den här diagramtypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata för diagrammet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Lägg till ett pajdiagram
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Ange diagrammets dataområde
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Demonstrera olika ChartSplitType‑värden
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Byt till en annan delningstyp
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Spara arbetsboken
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


