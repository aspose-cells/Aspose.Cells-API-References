---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageSaveOptions. Opzioni aggiuntive per la creazione dell'immagine"
type: docs
url: /it/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Opzioni aggiuntive per la creazione dell'immagine.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Osservazioni

Per un utilizzo avanzato, si prega di utilizzare [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) o [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageSaveOptionsPropertyImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Image Export");

            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;

            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pngOptions);
                Console.WriteLine("Image saved to memory stream successfully");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


