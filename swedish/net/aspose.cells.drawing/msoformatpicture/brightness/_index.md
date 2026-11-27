---
title: "MsoFormatPicture.Brightness"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture egenskap. Representerar ljusstyrkekorrigeringen för bilden i procentenheter"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Representerar ljusstyrkesmodifieringen för bilden i enhet av procent.

```csharp
public double Brightness { get; set; }
```

### Anmärkningar

Den ligger mellan -100% och 100%. Den fungerar på samma sätt som Excel 2007 eller senare versioner.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // Ställ in och hämta ljusstyrka
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // Ändra ljusstyrka
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


