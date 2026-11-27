---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageSaveOptions‑egenskap. Ytterligare alternativ för bildskapande"
type: docs
url: /sv/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Ytterligare alternativ för bildskapande.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Anmärkningar

För avancerad användning, använd [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) eller [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Exempel

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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


