---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di WorkbookPrintingPreview. La costruzione di WorkbookPrintingPreview"
type: docs
url: /it/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

Il costruttore di WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cartella di lavoro | Cartella di lavoro | Indicare quale cartella di lavoro deve essere stampata. |
| opzioni | ImageOrPrintOptions | ImageOrPrintOptions contiene alcune proprietà di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Impostare le opzioni di stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Creare l'anteprima di stampa con la cartella di lavoro e le opzioni
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Visualizzare il conteggio delle pagine
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Vedi anche

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


