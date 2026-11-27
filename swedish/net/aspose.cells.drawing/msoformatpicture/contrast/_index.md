---
title: "MsoFormatPicture.Contrast"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar kontrastmodifieringen för bilden i procentenheter"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Representerar kontrastmodifieringen för bilden.in enhet av procent.

```csharp
public double Contrast { get; set; }
```

### Anmärkningar

Den ligger mellan -100% och 100%. Den fungerar på samma sätt som Excel 2007 eller senare versioner.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyContrastDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            var picture = worksheet.Pictures[pictureIndex];

            // Ange och hämta kontrastvärdet
            picture.FormatPicture.Contrast = 50;
            Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);

            // Modifiera kontrast
            picture.FormatPicture.Contrast = 75;
            Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


