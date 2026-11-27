---
title: "ThreeDFormat.Material"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge det slutliga utseendet och känslan av en form"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutgiltiga utseendet och känslan av en form.

```csharp
public PresetMaterialType Material { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Åtkomst till ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt materialvärde
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Ställ in olika materialtyper och observera effekterna
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Konfigurera andra 3D-egenskaper för att bättre se materialeffekten
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Spara arbetsboken med 3D‑effekterna
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


