---
title: "ThreeDFormat.LightAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger vinkeln på extruderingsljusen"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Hämtar och anger vinkeln på extruderingsljusen.

```csharp
public double LightAngle { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Åtkomst till ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt LightAngle-värde
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Ställ in nytt LightAngle-värde (0 till 359,9 grader)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Konfigurera andra 3D-egenskaper för att se effekten av LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Spara arbetsboken för att se effekterna
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


