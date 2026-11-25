---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro (Visible)"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Imposta alcuni dati di esempio in entrambi i fogli
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Salva solo il secondo foglio usando SheetSet
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // Salva la cartella di lavoro con i fogli specificati
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


