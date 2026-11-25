---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Indica se verificare la compatibilità dei font per ogni carattere nel testo"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Indica se verificare la compatibilità del carattere per ogni carattere nel testo.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Osservazioni

Il valore predefinito è true. Disabilitare questa proprietà può migliorare le prestazioni. Tuttavia, quando il font predefinito o specificato per il testo/carattere non può essere usato per renderizzarlo, potrebbero comparire caratteri illeggibili (come blocchi) nel PDF generato. In tali situazioni l'utente dovrebbe mantenere questa proprietà impostata su true affinché venga cercato e utilizzato un font alternativo per renderizzare il testo invece;

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Crea le opzioni di salvataggio paginato
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Dimostra la proprietà CheckFontCompatibility
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Imposta le altre proprietà richieste
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Salva il documento con le opzioni specificate
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


