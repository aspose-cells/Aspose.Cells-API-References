---
title: "LowCodeImageSaveOptions.ImageOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeImageSaveOptions. Las opciones para renderizar imágenes"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/
---
## LowCodeImageSaveOptions.ImageOptions property

Las opciones para renderizar imágenes.

```csharp
public ImageOrPrintOptions ImageOptions { get; set; }
```

### Observaciones

Cuando se especifica una instancia de [`ImageOrPrintOptions`](../../../aspose.cells.rendering/imageorprintoptions/), el [`SaveFormat`](../saveformat/) será sobrescrito (si se había especificado antes).

### Ejemplos

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

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


