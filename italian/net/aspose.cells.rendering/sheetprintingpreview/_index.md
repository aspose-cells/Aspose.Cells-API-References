---
title: "Class SheetPrintingPreview"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.SheetPrintingPreview. Anteprima di stampa del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Anteprima di stampa del foglio di lavoro.

```csharp
public class SheetPrintingPreview
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | La costruzione di SheetPrintingPreview |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Valuta il conteggio totale delle pagine di questo foglio di lavoro |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Carica una cartella di lavoro esistente
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Crea un'istanza di SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Valuta e stampa il conteggio totale delle pagine del foglio di lavoro
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


