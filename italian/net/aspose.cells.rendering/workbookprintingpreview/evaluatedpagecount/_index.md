---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookPrintingPreview. Valuta il conteggio totale delle pagine di questo workbook"
type: docs
url: /it/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Valuta il conteggio totale delle pagine di questa cartella di lavoro

```csharp
public int EvaluatedPageCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Crea le opzioni di anteprima di stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crea l'anteprima di stampa del workbook
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Ottieni e visualizza il conteggio delle pagine valutato
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Vedi anche

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


