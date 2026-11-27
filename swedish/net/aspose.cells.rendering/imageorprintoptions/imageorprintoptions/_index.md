---
title: "ImageOrPrintOptions.ImageOrPrintOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Konstruktor.

```csharp
public ImageOrPrintOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Hello World!");
            
            // Demonstrera #ctor-användning
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Rendera bladet till bild
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            sheetRender.ToImage(0, "output.png");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


