---
title: "SparklineGroup.HorizontalAxisDateRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Rappresenta l'intervallo che contiene i valori di data per i dati della sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/
---
## SparklineGroup.HorizontalAxisDateRange property

Rappresenta l'intervallo che contiene i valori di data per i dati della sparkline.

```csharp
public string HorizontalAxisDateRange { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di data e valore per la sparkline
            sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
            sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
            sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
            
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["D2"].PutValue(3);

            // Definisci l'CellArea dove verrà posizionata la sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 1,
                EndRow = 1
            };

            // Aggiungi un gruppo di sparkline con asse delle date
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Imposta l'intervallo di date per l'asse orizzontale
            group.HorizontalAxisDateRange = "A1:D1";
            group.ShowHorizontalAxis = true;

            // Salva la cartella di lavoro
            workbook.Save("SparklineWithDateAxis.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


