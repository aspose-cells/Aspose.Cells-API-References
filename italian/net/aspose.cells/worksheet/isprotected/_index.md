---
title: "Worksheet.IsProtected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se il foglio di lavoro è protetto"
type: docs
url: /it/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Indica se il foglio di lavoro è protetto.

```csharp
public bool IsProtected { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Proteggi il workbook e il primo foglio di lavoro
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Verifica se il foglio di lavoro è protetto
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Salva la cartella di lavoro
            workbook.Save("protected_worksheet.xlsx");

            // Carica la cartella di lavoro salvata e verifica la protezione
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


