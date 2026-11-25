---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere un errore nel rendering di forme, immagini, grafici, ecc."
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere relativo a forme, immagini, rendering di grafici, ecc.

```csharp
public bool IgnoreError { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio con potenziali errori di formattazione
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Imposta IgnoreError su true per ignorare eventuali errori di conversione
            options.IgnoreError = true;
            
            // Salva la cartella di lavoro come PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


