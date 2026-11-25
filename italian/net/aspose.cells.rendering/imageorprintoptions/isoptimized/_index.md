---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica se ottimizzare gli elementi di output"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Indica se ottimizzare gli elementi di output.

```csharp
public bool IsOptimized { get; set; }
```

### Osservazioni

Il valore predefinito è false. Attualmente, quando questa proprietà è impostata su true, vengono eseguite le seguenti ottimizzazioni: 1. ottimizzare le linee di bordo. 2. ottimizzare la dimensione del file durante il rendering in immagine Svg.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Configura le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Dimostra la proprietà IsOptimized
            options.IsOptimized = true; // Enable optimization
            
            // Esegui il rendering del foglio in immagine
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


