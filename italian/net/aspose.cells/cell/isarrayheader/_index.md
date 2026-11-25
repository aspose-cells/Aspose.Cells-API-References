---
title: "Cell.IsArrayHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica che la formula della cella è una formula di array ed è la prima cella dell'array"
type: docs
url: /it/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indica che la formula della cella è una formula array ed è la prima cella dell'array.

```csharp
public bool IsArrayHeader { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una formula di array nell'intervallo B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Verifica e stampa la proprietà IsArrayHeader
            // Nota: IsArrayHeader è di sola lettura e viene impostato automaticamente per le intestazioni di formule di array
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


