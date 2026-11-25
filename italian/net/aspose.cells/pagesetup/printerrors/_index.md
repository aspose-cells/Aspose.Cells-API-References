---
title: "PageSetup.PrintErrors"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Specifica il tipo di errore di stampa visualizzato"
type: docs
url: /it/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Specifica il tipo di errore di stampa visualizzato.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Imposta gli errori di stampa per visualizzarli come vuoti
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Modifica gli errori di stampa per visualizzarli come trattini
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Salva la cartella di lavoro
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


