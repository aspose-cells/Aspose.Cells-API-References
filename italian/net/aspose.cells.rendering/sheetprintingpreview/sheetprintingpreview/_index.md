---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore SheetPrintingPreview. La costruzione di SheetPrintingPreview"
type: docs
url: /it/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

La costruzione di SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| foglio | Worksheet | Indica quale foglio di calcolo deve essere stampato. |
| opzioni | ImageOrPrintOptions | ImageOrPrintOptions contiene alcune proprietà di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crea opzioni di immagine/stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Crea l'anteprima di stampa del foglio
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Restituisci il conteggio delle pagine valutato
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


