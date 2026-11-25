---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Quando i caratteri in Excel sono Unicode e non viene impostato il font corretto nello stile della cella, possono apparire come blocchi nell'immagine PDF. Imposta la proprietà DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito di sistema per visualizzare questi caratteri Unicode."
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode.

```csharp
public string DefaultFont { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi testo di esempio alla cella
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // Crea le opzioni immagine e imposta il font predefinito
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // Renderizza il foglio di lavoro in immagine
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


