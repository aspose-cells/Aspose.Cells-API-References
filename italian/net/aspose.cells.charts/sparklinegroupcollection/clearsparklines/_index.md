---
title: "SparklineGroupCollection.ClearSparklines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SparklineGroupCollection. Cancella gli sparkline che si trovano all'interno di un'area di celle"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Cancella le sparkline che si trovano all'interno di un'area di celle.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | Specifica l'area di celle. |

### Osservazioni

[`SparklineGroup`](../../sparklinegroup/) will be removed too if it does not contains any [`Sparkline`](../../sparkline/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            try
            {
                // Chiama il metodo ClearSparklines con il parametro CellArea
                sheet.SparklineGroups.ClearSparklines(ca);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


