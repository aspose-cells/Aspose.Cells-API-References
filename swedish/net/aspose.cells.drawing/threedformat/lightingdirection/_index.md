---
title: "ThreeDFormat.LightingDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger riktningen från vilken ljusriggen är orienterad i förhållande till scenen"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Hämtar och anger riktningen från vilken ljusanordningen är orienterad i förhållande till scenen.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Hämta ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Ställ in initiala 3D-egenskaper
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Visa den aktuella belysningsriktningen
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Ändra belysningsriktning och observera effekterna
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Byt till en annan riktning
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Spara arbetsboken för att se de visuella effekterna
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


