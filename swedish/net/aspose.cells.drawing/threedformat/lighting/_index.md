---
title: "ThreeDFormat.Lighting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger typ av ljusrigg"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Hämtar och anger typen av ljusanordning.

```csharp
public LightRigType Lighting { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Hämta ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt ljusvärde
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Ställ in olika typer av belysning och observera effekterna
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Applicera några andra 3D-egenskaper för att bättre se belysningseffekten
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Spara med den första belysningstypen
            workbook.Save("BrightRoomLighting.xlsx");

            // Byt till en annan belysningstyp
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Byt till en tredje belysningstyp
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Se även

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


