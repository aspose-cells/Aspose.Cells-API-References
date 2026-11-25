---
title: "PageSetup.FirstPageNumber"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta il numero della prima pagina che verrà usato quando questo foglio viene stampato"
type: docs
url: /it/net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Rappresenta il numero di pagina iniziale che verrà usato quando questo foglio viene stampato.

```csharp
public int FirstPageNumber { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFirstPageNumberDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le proprietà di configurazione della pagina
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            
            // Stampa i risultati
            Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


