---
title: "ImageOrPrintOptions.PageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il numero di pagine da salvare"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Ottiene o imposta il numero di pagine da salvare.

```csharp
public int PageCount { get; set; }
```

### Osservazioni

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine verranno renderizzate.

### Esempi

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Page 1 Data");
            worksheet.Cells["A2"].PutValue("Sample Content");
            worksheet.Cells["A3"].PutValue("Demo for PageCount");
            
            // Imposta l'area di stampa e la configurazione della pagina
            worksheet.PageSetup.PrintArea = "A1:A3";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
            options.OnlyArea = true;

            // Renderizza il foglio di lavoro in immagine
            SheetRender renderer = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Salva l'immagine su file
                string outputPath = "output.png";
                File.WriteAllBytes(outputPath, stream.ToArray());
                Console.WriteLine($"Output saved to: {outputPath}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


