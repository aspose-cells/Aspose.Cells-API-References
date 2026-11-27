---
title: "Picture.ImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar bildformatet för bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Hämtar bildformatet för bilden.

```csharp
public ImageType ImageType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyImageTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Infoga första bilden (PNG)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);

            // Infoga andra bilden (JPEG)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
        }
    }
}
```

### Se även

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


