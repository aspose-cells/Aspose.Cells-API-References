---
title: "Worksheet.DisplayRightToLeft"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la visualizzazione da destra a sinistra
            worksheet.DisplayRightToLeft = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output.ods");
            
            // Ricarica la cartella di lavoro per verificare l'impostazione
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


