---
title: "ThreeDFormat.LightAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit l'angle des lumières d'extrusion"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Obtient et définit l'angle des lumières d'extrusion.

```csharp
public double LightAngle { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Accéder au ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Affichez la valeur actuelle de LightAngle
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Définissez une nouvelle valeur de LightAngle (0 à 359,9 degrés)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Configurez d'autres propriétés 3D pour voir l'effet de LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Enregistrer le classeur pour voir les effets
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


