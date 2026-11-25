---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indica che l'altezza della riga e l'altezza del carattere predefinito corrispondono"
type: docs
url: /it/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Imposta e dimostra la proprietà IsDefaultRowHeightMatched
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


