---
title: "ImageOrPrintOptions.Quality"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato JPEG. Il valore predefinito è 100"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. Il valore predefinito è 100

```csharp
public int Quality { get; set; }
```

### Osservazioni

Ha effetto solo quando si salva in JPEG. Il valore deve essere compreso tra 0 e 100. Il valore predefinito è 100.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Creare opzioni immagine con impostazioni di qualità diverse
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Renderizzare il foglio di lavoro in immagine ad alta qualità
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Modificare la qualità per dimostrare la differenza
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


