---
title: "ImageOrPrintOptions.OnePagePerSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida e le altre impostazioni di pagesetup avranno comunque effetto"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. Il formato carta di pagesetup sarà invalido, ma le altre impostazioni di pagesetup continueranno ad avere effetto.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
            }

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true; // Key property being demonstrated
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crea il rendering del foglio
            SheetRender sr = new SheetRender(worksheet, options);
            
            // Salva l'immagine di output
            sr.ToImage(0, "OnePagePerSheetOutput.png");
            
            Console.WriteLine("Output saved with OnePagePerSheet=true");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


