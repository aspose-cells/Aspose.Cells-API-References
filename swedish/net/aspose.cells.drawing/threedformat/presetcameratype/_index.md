---
title: "ThreeDFormat.PresetCameraType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger den förinställda kameratypen för extrudering"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

Hämtar och anger den förinställda kameratypen för extrusion.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // Hämta ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa det aktuella PresetCameraType‑värdet
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // Ange ett nytt PresetCameraType‑värde
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // Applicera ytterligare 3D‑formatering för att göra effekten synlig
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Visa det nya PresetCameraType‑värdet
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // Spara arbetsboken för att visa effekten
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


