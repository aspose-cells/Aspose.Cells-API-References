---
title: "Cells.FirstCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar den första cellen i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Hämtar den första cellen i detta kalkylblad.

```csharp
public Cell FirstCell { get; }
```

### Anmärkningar

Returnerar null om det inte finns någon data i kalkylbladet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Hämta cellsamling
            Cells cells = worksheet.Cells;
            
            // Demonstrera FirstCell-egenskapen
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // Skapa diagram med FirstCell och LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Spara arbetsboken
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


