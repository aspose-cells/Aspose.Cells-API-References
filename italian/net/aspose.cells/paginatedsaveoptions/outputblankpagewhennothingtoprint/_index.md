---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Indica se generare una pagina vuota quando non c'è nulla da stampare"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Indica se generare una pagina vuota quando non c'è nulla da stampare.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e nascondilo (simulando l'assenza di contenuti da stampare)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // Imposta le opzioni di salvataggio PDF con OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Salva in PDF - non dovrebbe essere generata alcuna pagina vuota
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Modifica l'opzione a true
            options.OutputBlankPageWhenNothingToPrint = true;

            // Salva di nuovo - dovrebbe essere generata una pagina vuota
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


