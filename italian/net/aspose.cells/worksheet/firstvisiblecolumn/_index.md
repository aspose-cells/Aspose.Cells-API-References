---
title: "Worksheet.FirstVisibleColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta l'indice della prima colonna visibile"
type: docs
url: /it/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Rappresenta l'indice della prima colonna visibile.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nascondi la prima colonna (indice 0)
            worksheet.Cells.HideColumn(0);
            
            // Ottieni e visualizza l'indice della prima colonna visibile
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Salva la cartella di lavoro
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


