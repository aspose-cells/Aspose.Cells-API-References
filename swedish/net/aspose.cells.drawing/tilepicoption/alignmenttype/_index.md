---
title: "TilePicOption.AlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TilePicOption-egenskap. Hämtar eller anger justeringen för kakling"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Hämtar eller anger justeringen för kakling.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel för att demonstrera mosaik
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Konfigurera fyllningsformatet för att använda en kaklad bild
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Skapa och konfigurera TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Visa initialt AlignmentType-värde
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Ställ in justeringen till TopRight
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Tillämpa kakelalternativ på formens fyllning
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Läs in exempelbild (1×1-pixel röd prick)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Spara modifierad arbetsbok
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Ändra justeringen till BottomLeft och spara en annan version
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Se även

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


