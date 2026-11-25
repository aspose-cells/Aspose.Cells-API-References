---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. True indica che l'intestazione/piè di pagina delle pagine dispari è diversa rispetto a quelle pari"
type: docs
url: /it/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True indica che l'intestazione/piè di pagina delle pagine dispari è diversa dalle pagine dispari.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Abilita intestazioni/piè di pagina diversi per le pagine dispari e pari
            pageSetup.IsHFDiffOddEven = true;
            
            // Imposta piè di pagina diversi per le pagine dispari e pari
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Verifica le impostazioni caricando il file salvato
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


