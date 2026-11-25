---
title: "Cells.FirstCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene la prima cella in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Ottiene la prima cella in questo foglio di lavoro.

```csharp
public Cell FirstCell { get; }
```

### Osservazioni

Restituisce null se non ci sono dati nel foglio di lavoro.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Ottieni la raccolta di celle
            Cells cells = worksheet.Cells;
            
            // Dimostra la proprietà FirstCell
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // Crea un grafico usando FirstCell e LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Salva la cartella di lavoro
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


