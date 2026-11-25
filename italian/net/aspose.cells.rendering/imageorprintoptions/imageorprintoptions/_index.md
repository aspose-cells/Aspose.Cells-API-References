---
title: "ImageOrPrintOptions.ImageOrPrintOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ImageOrPrintOptions. Ctor"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Ctor.

```csharp
public ImageOrPrintOptions()
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Hello World!");
            
            // Dimostra l'uso di #ctor
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Esegui il rendering del foglio in immagine
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            sheetRender.ToImage(0, "output.png");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


