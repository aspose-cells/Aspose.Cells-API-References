---
title: "LowCodeImageSaveOptions.ImageOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeImageSaveOptions‑egenskap. Alternativen för att rendera bilder"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/
---
## LowCodeImageSaveOptions.ImageOptions property

Alternativen för att rendera bilder.

```csharp
public ImageOrPrintOptions ImageOptions { get; set; }
```

### Anmärkningar

När en [`ImageOrPrintOptions`](../../../aspose.cells.rendering/imageorprintoptions/)‑instans är specificerad, kommer [`SaveFormat`](../saveformat/) att skrivas över (om den tidigare har angetts).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Output");

            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.ImageOptions = new ImageOrPrintOptions();

            Console.WriteLine("Default Horizontal Resolution: " + saveOptions.ImageOptions.HorizontalResolution);
            
            saveOptions.ImageOptions.HorizontalResolution = 300;
            saveOptions.ImageOptions.VerticalResolution = 300;
            SheetRender highResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            highResRenderer.ToImage(0, "HighResolutionOutput.png");

            saveOptions.ImageOptions.HorizontalResolution = 150;
            saveOptions.ImageOptions.VerticalResolution = 150;
            SheetRender lowResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            lowResRenderer.ToImage(0, "LowResolutionOutput.png");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


