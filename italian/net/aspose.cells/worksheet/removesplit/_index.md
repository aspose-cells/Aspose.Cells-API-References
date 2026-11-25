---
title: "Worksheet.RemoveSplit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet method. Rimuove la finestra divisa"
type: docs
url: /it/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Rimuove la divisione della finestra.

```csharp
public void RemoveSplit()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dividi il foglio di lavoro
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Rimuovi la divisione
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


