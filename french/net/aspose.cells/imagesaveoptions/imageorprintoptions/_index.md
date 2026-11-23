---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageSaveOptions. Options supplémentaires de création d'image"
type: docs
url: /fr/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Options supplémentaires de création d’image.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Remarques

Pour une utilisation avancée, veuillez utiliser [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) ou [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Exemples

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

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


