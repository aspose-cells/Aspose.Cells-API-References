---
title: "Worksheet.ClearComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Cancella tutti i commenti nel foglio di calcolo del designer"
type: docs
url: /it/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Cancella tutti i commenti nel foglio di calcolo del designer.

```csharp
public void ClearComments()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi commenti di esempio alle celle usando i riferimenti delle celle
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Mostra il conteggio dei commenti prima della cancellazione
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Cancella tutti i commenti dal foglio di lavoro
            worksheet.ClearComments();

            // Mostra il conteggio dei commenti dopo la cancellazione
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Salva la cartella di lavoro
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


