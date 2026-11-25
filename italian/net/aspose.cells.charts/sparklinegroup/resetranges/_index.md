---
title: "SparklineGroup.ResetRanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SparklineGroup. Reimposta l'intervallo dei dati e l'intervallo di posizione del gruppo di sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Reimposta l'intervallo di dati e l'intervallo di posizione del gruppo di sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataRange | String | Specifica il nuovo intervallo di dati del gruppo di sparkline. |
| isVertical | Booleano | Specifica se tracciare le sparklines dal nuovo intervallo di dati per riga o per colonna. |
| locationRange | CellArea | Specifica dove posizionare le sparklines. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
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

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Prepara i parametri per ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Chiama ResetRanges con i parametri (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


