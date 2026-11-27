---
title: "MsoFormatPicture.Gamma"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar bildens gamma"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Representerar gamma för bilden.

```csharp
public double Gamma { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en bild i kalkylbladet (använd en exempelbildsökväg)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Åtkomst till MsoFormatPicture‑objektet
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Ställ in Gamma-egenskapen
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Spara arbetsboken
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


