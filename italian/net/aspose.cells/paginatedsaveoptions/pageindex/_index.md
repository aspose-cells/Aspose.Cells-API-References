---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta l'indice basato su 0 della prima pagina da salvare"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Ottiene o imposta l'indice basato su 0 della prima pagina da salvare.

```csharp
public int PageIndex { get; set; }
```

### Osservazioni

Il valore predefinito è 0.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio su più pagine
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // Imposta le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Imposta per stampare le pagine 3-4 (indice basato su 0)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Salva il PDF con le pagine selezionate
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


