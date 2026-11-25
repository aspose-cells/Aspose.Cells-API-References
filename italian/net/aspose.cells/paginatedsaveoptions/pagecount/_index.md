---
title: "PaginatedSaveOptions.PageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta il numero di pagine da salvare"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Ottiene o imposta il numero di pagine da salvare.

```csharp
public int PageCount { get; set; }
```

### Osservazioni

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine verranno renderizzate..

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Apri un file Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Inizializza le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Imposta per stampare solo 2 pagine a partire dalla pagina 4 (indice basato su 0 è 3)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Salva il file PDF
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


