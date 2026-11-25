---
title: "Workbook.AcceptAllRevisions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Accetta tutte le modifiche tracciate nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accetta tutte le modifiche tracciate nella cartella di lavoro.

```csharp
public void AcceptAllRevisions()
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcune revisioni (il tracciamento delle modifiche deve essere abilitato in Excel prima)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Salva con revisioni
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Riapri la cartella di lavoro
            workbook = new Workbook(sourcePath);
            
            // Verifica se ci sono revisioni e accettale
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Salva senza revisioni
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


