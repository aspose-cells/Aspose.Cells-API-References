---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageSaveOptions. Opciones adicionales de creación de imágenes"
type: docs
url: /es/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Opciones adicionales de creación de imagen.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Observaciones

Para uso avanzado, por favor use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) o [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Ejemplos

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

### Ver también

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


