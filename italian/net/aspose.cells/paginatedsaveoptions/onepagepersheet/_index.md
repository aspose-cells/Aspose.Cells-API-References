---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida e le altre impostazioni di pagesetup avranno comunque effetto"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. Il formato carta di pagesetup sarà invalido, ma le altre impostazioni di pagesetup continueranno ad avere effetto.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Aggiungi alcuni dati di esempio a entrambi i fogli
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // Imposta le opzioni di salvataggio PDF con OnePagePerSheet
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Salva la cartella di lavoro in PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


