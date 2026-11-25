---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene interruzioni di pagina automatiche"
type: docs
url: /it/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Ottiene le interruzioni di pagina automatiche.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | ImageOrPrintOptions | Le opzioni di stampa |

### Valore di ritorno

Le aree delle interruzioni di pagina automatiche.

### Osservazioni

Ogni area di cella rappresenta un foglio.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare interruzioni di pagina
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Imposta l'area di stampa e la configurazione della pagina
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Ottieni le interruzioni di pagina con ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // Restituisci le informazioni della prima interruzione di pagina
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


