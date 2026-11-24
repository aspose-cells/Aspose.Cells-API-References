---
title: "ThreeDFormat.Material"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Stellt das voreingestellte Material dar, das mit den Lichteigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen."
type: docs
url: /de/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Stellt das voreingestellte Material dar, das mit den Lichteigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen.

```csharp
public PresetMaterialType Material { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Greife auf das ThreeDFormat der Form zu.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Aktuellen Materialwert anzeigen
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Verschiedene Materialtypen festlegen und die Effekte beobachten
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Weitere 3D-Eigenschaften konfigurieren, um den Materialeffekt besser zu sehen
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Arbeitsmappe mit den 3D-Effekten speichern
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


