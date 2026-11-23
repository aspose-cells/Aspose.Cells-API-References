---
title: "ThreeDFormat.Lighting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit le type du dispositif d'éclairage"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Obtient et définit le type de dispositif d'éclairage.

```csharp
public LightRigType Lighting { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Obtenir le ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur d'éclairage actuelle
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Définissez différents types d'éclairage et observez les effets
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Appliquez d'autres propriétés 3D pour mieux voir l'effet d'éclairage
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Enregistrez avec le premier type d'éclairage
            workbook.Save("BrightRoomLighting.xlsx");

            // Changez pour un autre type d'éclairage
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Changez pour un troisième type d'éclairage
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


