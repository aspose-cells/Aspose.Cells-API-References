---
title: "Picture.OriginalHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar originalhöjden på bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Hämtar bildens ursprungliga höjd.

```csharp
public int OriginalHeight { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Hämta och visa originalhöjden på bilden
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // Spara arbetsboken
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


