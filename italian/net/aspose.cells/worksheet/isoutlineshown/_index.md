---
title: "Worksheet.IsOutlineShown"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se mostrare l'outline"
type: docs
url: /it/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Indica se mostrare la struttura.

```csharp
public bool IsOutlineShown { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la visualizzazione dell'outline
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Salva e ricarica per dimostrare la persistenza
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


