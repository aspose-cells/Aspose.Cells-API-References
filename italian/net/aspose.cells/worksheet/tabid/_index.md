---
title: "Worksheet.TabId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Specifica l'identificatore interno per il foglio"
type: docs
url: /it/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Specifica l'identificatore interno per il foglio.

```csharp
public int TabId { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la proprietà TabId
            worksheet.TabId = 107;
            
            // Salva la cartella di lavoro
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Carica la cartella di lavoro salvata per verificare il TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visualizza il valore del TabId
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


