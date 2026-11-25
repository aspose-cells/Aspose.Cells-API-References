---
title: "PageSetup.IsAutoFirstPageNumber"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Indica se il numero della prima pagina è assegnato automaticamente"
type: docs
url: /it/net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

Indica se il numero della prima pagina viene assegnato automaticamente.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutoFirstPageNumberDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le proprietà di configurazione della pagina
            worksheet.PageSetup.IsAutoFirstPageNumber = true;
            Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);

            // Aggiungi un secondo foglio di lavoro
            worksheet = workbook.Worksheets.Add("Sheet2");
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


