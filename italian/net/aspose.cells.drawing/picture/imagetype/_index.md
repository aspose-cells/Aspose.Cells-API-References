---
title: "Picture.ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene il formato immagine dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Ottiene il formato immagine dell'immagine.

```csharp
public ImageType ImageType { get; }
```

### Esempi

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

            // Inserisci la prima immagine (PNG)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);

            // Inserisci la seconda immagine (JPEG)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
        }
    }
}
```

### Vedi anche

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


