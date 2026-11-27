---
title: "MsoFormatPicture.TransparentColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Hämtar och anger den transparenta färgen för bilden"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Hämtar och anger den transparenta färgen för bilden.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparentColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelbild (använd en rektangel med en solid färg som exempel)
            int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ange transparent färg
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.Blue;
            picture.FormatPicture.TransparentColor = transparentColor;

            // Hämta och visa den transparenta färgen
            CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
            Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);

            // Spara arbetsboken
            workbook.Save("TransparentColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


