---
title: "Classe WorkbookPrintingPreview"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.WorkbookPrintingPreview. Anteprima di stampa della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Anteprima di stampa della cartella di lavoro.

```csharp
public class WorkbookPrintingPreview
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | Il costruttore di WorkbookPrintingPreview |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Valuta il conteggio totale delle pagine di questa cartella di lavoro |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Carica una cartella di lavoro esistente
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Crea un'istanza di ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Crea un'istanza di WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Valuta il conteggio totale delle pagine della cartella di lavoro
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Stampa il conteggio delle pagine valutato
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


