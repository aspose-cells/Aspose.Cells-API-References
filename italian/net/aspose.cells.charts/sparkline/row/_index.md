---
title: "Sparkline.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Sparkline. Restituisce l'indice di riga dello sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Ottiene l'indice di riga dello sparkline.

```csharp
public int Row { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Aggiungi sparkline alla riga 0, colonna 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Visualizza la posizione della riga (proprietà di sola lettura)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Per modificare la posizione, è necessario rimuovere e ricreare lo sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Salva cartella di lavoro
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


