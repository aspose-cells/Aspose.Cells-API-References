---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageSaveOptions-Eigenschaft. Zusätzliche Optionen zur Bildgenerierung"
type: docs
url: /de/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Zusätzliche Bild-Erstellungsoptionen.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Hinweise

Für erweiterte Anwendungsfälle verwenden Sie bitte [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) oder [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Beispiele

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

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


