---
title: "PageSetup.IsHFDiffFirst"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine"
type: docs
url: /it/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta intestazioni/piè di pagina diversi per la prima pagina
            pageSetup.IsHFDiffFirst = true;
            
            // Imposta intestazioni/piè di pagina
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Ricarica la cartella di lavoro per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Verifica dell'output
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


