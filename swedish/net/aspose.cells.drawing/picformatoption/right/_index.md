---
title: "PicFormatOption.Right"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption-egenskap. Hämtar eller anger det högra offsetet för att sträcka bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Hämtar eller anger det högra offsetet för att sträcka bilden.

```csharp
public double Right { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med angivna dimensioner
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Konfigurera bildfyllning för formen
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // Kom åt bildformatalternativ via TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Visa och ändra Right-egenskapen
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Verifiera det nya värdet och spara ändringarna
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


