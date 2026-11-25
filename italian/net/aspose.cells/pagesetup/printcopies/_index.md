---
title: "PageSetup.PrintCopies"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Ottiene e imposta il numero di copie da stampare"
type: docs
url: /it/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Ottiene e imposta il numero di copie da stampare.

```csharp
public int PrintCopies { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il numero di copie di stampa a 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Visualizza l'impostazione corrente delle copie di stampa
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


