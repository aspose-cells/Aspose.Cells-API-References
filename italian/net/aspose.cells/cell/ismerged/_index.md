---
title: "Cell.IsMerged"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Verifica se una cella fa parte di un intervallo unito o meno"
type: docs
url: /it/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Verifica se una cella fa parte di un intervallo unito o meno.

```csharp
public bool IsMerged { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Unisci le celle da A1 a B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Verifica se la cella A1 è unita
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Verifica se la cella C1 è unita (dovrebbe essere falso)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Salva la cartella di lavoro
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


