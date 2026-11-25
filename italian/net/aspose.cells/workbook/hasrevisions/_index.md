---
title: "Workbook.HasRevisions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Restituisce se la cartella di lavoro ha modifiche tracciate"
type: docs
url: /it/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Ottiene se il workbook ha modifiche tracciate

```csharp
public bool HasRevisions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Apporta una modifica che creerà una revisione
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Verifica se il workbook ha revisioni
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Accetta tutte le revisioni (se presenti)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Verifica nuovamente dopo aver accettato le revisioni
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


