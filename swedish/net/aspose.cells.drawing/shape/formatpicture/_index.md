---
title: "Shape.FormatPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger alternativen för bildformatet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Hämtar och anger alternativen för bildformatet.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Åtkomst till shape's FormatPicture-egenskap
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Ändra bildformatets egenskaper
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Spara arbetsboken
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


