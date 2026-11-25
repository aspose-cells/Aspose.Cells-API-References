---
title: "Worksheet.UniqueId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene e imposta l'ID univoco, è lo stesso di 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /it/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Ottiene e imposta l'ID univoco, è lo stesso di {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Genera un ID univoco per il foglio di lavoro
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Imposta la proprietà UniqueId del primo foglio di lavoro
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Salva la cartella di lavoro
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Ricarica la cartella di lavoro per verificare che l'UniqueId persista
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Emetti l'UniqueId per dimostrare la funzionalità
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


