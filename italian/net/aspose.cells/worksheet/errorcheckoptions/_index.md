---
title: "Worksheet.ErrorCheckOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Restituisce l'impostazione di controllo errori applicata a determinati intervalli"
type: docs
url: /it/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Ottiene l'impostazione di controllo errori applicata su alcuni intervalli.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Abilita le opzioni di controllo errori
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Ottieni il conteggio degli intervalli per l'opzione
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Salva la cartella di lavoro
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


