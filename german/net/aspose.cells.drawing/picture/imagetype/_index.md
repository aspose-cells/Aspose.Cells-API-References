---
title: "Picture.ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt das Bildformat des Bildes zurück"
type: docs
url: /de/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Ermittelt das Bildformat des Bildes.

```csharp
public ImageType ImageType { get; }
```

### Beispiele

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

            // Füge das erste Bild ein (PNG)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);

            // Füge das zweite Bild ein (JPEG)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
        }
    }
}
```

### Siehe auch

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


