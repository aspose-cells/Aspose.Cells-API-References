---
title: "Sparkline.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Sparkline. Ottiene l'indice di colonna della sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Ottiene l'indice di colonna dello sparkline.

```csharp
public int Column { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Aggiungi una sparkline nella colonna 4 e dimostra la proprietà Column
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Visualizza la proprietà column (sola lettura)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // Per modificare la posizione della colonna, è necessario rimuovere e ri‑aggiungere la sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Salva cartella di lavoro
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


