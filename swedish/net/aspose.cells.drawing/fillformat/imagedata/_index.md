---
title: "FillFormat.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar och anger bilddata"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Hämtar och anger bildens bilddata.

```csharp
public byte[] ImageData { get; set; }
```

### Anmärkningar

Om fyllningsformatet inte är ett anpassat texturformat, returneras null.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempelbild i kalkylbladet
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Skapa en kommentar och ange bilddata
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Spara arbetsbok
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


