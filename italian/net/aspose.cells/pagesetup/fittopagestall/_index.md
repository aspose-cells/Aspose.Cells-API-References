---
title: "PageSetup.FitToPagesTall"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1"
type: docs
url: /it/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Rappresenta il numero di pagine in altezza a cui il foglio di lavoro verrà scalato quando viene stampato. Il valore predefinito è 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Osservazioni

Devi impostare FitToPagesWide a zero se vuoi adattare tutte le righe su una sola pagina.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per far sì che il foglio si estenda su più pagine
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // Ottieni l'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta l'area di stampa
            pageSetup.PrintArea = "A1:J100";
            
            // Imposta la proprietà FitToPagesTall per adattare tutte le righe su una pagina
            pageSetup.FitToPagesTall = 1;
            
            // Imposta la proprietà FitToPagesWide per adattare tutte le colonne su una pagina
            pageSetup.FitToPagesWide = 1;
            
            // Imposta la dimensione della carta
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Stampa le linee della griglia
            pageSetup.PrintGridlines = true;

            // Crea le opzioni di rendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crea il renderer del foglio
            SheetRender render = new SheetRender(worksheet, options);
            
            // Restituisci la scala della pagina
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


