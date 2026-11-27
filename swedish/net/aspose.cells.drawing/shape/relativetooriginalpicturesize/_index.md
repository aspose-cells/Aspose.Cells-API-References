---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om figuren är relativ till originalbildens storlek"
type: docs
url: /sv/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Anger om figuren är relativ till bildens ursprungliga storlek.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Åtkomst till figurens egenskaper – Bild är redan en Shape, ingen behov av att kasta
            Shape shape = picture;

            // Demonstrera RelativeToOriginalPictureSize-egenskapen
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Ändra egenskapen
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


