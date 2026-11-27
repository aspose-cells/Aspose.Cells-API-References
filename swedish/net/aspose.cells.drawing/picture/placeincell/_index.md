---
title: "Picture.PlaceInCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-metoden. Placera den här bilden i cellen"
type: docs
url: /sv/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Placera den här bilden i cellen

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället Picture.IsPlacedInCell property. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Placera bilden i cell A1
            picture.PlaceInCell();

            // Verifiera att bilden är placerad i cellen
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


