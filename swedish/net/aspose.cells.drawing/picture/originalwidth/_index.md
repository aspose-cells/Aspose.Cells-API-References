---
title: "Picture.OriginalWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar den ursprungliga bredden på bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Hämtar bildens ursprungliga bredd.

```csharp
public int OriginalWidth { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Hämta och visa den ursprungliga bredden på bilden
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

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


