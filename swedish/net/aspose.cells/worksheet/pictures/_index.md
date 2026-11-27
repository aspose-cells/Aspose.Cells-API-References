---
title: "Worksheet.Pictures"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Hämtar en Picture‑samling"
type: docs
url: /sv/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Hämtar en [`Picture`](../../../aspose.cells.drawing/picture/) samling.

```csharp
public PictureCollection Pictures { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ställ in Picture‑egenskaper
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### Se även

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


