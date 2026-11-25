---
title: "PaginatedSaveOptions.AllColumnsInOnePagePerSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà output su una sola pagina nel risultato. La larghezza della dimensione della carta di pagesetup sarà ignorata e le altre impostazioni di pagesetup avranno ancora effetto"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza del formato carta di pagesetup verrà ignorata, mentre le altre impostazioni di pagesetup continueranno ad avere effetto.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare l'adattamento delle colonne
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[0, i].PutValue("Column " + (i + 1));
                worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
            }

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;

            // Salva la cartella di lavoro con le opzioni
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with all columns in one page per sheet.");
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


