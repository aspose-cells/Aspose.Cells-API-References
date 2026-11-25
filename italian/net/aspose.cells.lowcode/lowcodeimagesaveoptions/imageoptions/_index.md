---
title: "LowCodeImageSaveOptions.ImageOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeImageSaveOptions. Le opzioni per il rendering delle immagini"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/
---
## LowCodeImageSaveOptions.ImageOptions property

Le opzioni per il rendering delle immagini.

```csharp
public ImageOrPrintOptions ImageOptions { get; set; }
```

### Osservazioni

Quando è specificata un'istanza di [`ImageOrPrintOptions`](../../../aspose.cells.rendering/imageorprintoptions/), il [`SaveFormat`](../saveformat/) verrà sovrascritto (se era stato specificato in precedenza).

### Esempi

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

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


