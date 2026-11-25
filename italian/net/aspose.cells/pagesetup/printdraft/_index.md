---
title: "PageSetup.PrintDraft"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta se il foglio verrà stampato senza grafica"
type: docs
url: /it/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Rappresenta se il foglio verrà stampato senza grafica.

```csharp
public bool PrintDraft { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi all'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta la proprietà PrintDraft su true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Modifica la proprietà PrintDraft su false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


