---
title: "SheetSet.Active"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SheetSet. Ottiene un set con il foglio attivo della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Ottiene un insieme con il foglio attivo della cartella di lavoro.

```csharp
public static SheetSet Active { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Imposta il secondo foglio di lavoro come attivo
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Aggiungi dati a entrambi i fogli di lavoro
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Salva solo il foglio attivo
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Salva tutti i fogli per il confronto
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


