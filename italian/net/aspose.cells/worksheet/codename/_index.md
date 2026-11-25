---
title: "Worksheet.CodeName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene il nome codice del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Ottiene il nome codice del foglio di lavoro.

```csharp
public string CodeName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Visualizza il CodeName predefinito
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Modifica il CodeName
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Aggiungi un nuovo foglio di lavoro e mostra il suo CodeName
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


