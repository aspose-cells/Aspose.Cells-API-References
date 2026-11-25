---
title: "Worksheet.CellWatches"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la raccolta di celle su questo foglio di lavoro monitorate nella finestra di osservazione"
type: docs
url: /it/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Ottiene la collezione di celle di questo foglio di lavoro monitorate nella 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alla cella B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Aggiungi monitoraggio cella per B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Visualizza le informazioni di monitoraggio
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Salva la cartella di lavoro
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


