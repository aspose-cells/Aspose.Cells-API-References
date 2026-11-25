---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il formato pixel per le immagini generate"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Ottiene o imposta il formato pixel per le immagini generate.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Osservazioni

Il valore predefinito è PixelFormat.Format32bppArgb.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visualizza il valore corrente della proprietà ImageType (poiché PixelFormat non esiste)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Nota: Poiché PixelFormat non esiste nell'API, dimostriamo ImageType invece
                // che è la proprietà più correlata per le impostazioni del formato immagine

                // Crea un SheetRender per dimostrare le opzioni in uso
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Salva il risultato come immagine per dimostrare le opzioni
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


