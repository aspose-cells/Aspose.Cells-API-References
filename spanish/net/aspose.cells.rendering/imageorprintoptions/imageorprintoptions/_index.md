---
title: "ImageOrPrintOptions.ImageOrPrintOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor ImageOrPrintOptions. Ctor"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Ctor.

```csharp
public ImageOrPrintOptions()
```

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Hello World!");
            
            // Demostrar el uso de #ctor
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Renderizar la hoja a imagen
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            sheetRender.ToImage(0, "output.png");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


