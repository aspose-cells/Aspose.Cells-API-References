---
title: "ExternalLink.IsReferred"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalLink. Indica se questo collegamento esterno è referenziato da altri"
type: docs
url: /it/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Indica se questo collegamento esterno è referenziato da altri.

```csharp
public bool IsReferred { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con collegamento esterno
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi riferimento al collegamento esterno
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Verifica se il collegamento esterno è referenziato
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


