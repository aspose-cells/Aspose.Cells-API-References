---
title: "ThreeDFormat.RotationY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la rotation de la forme extrudée autour de l'axe y en degrés"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Obtient et définit la rotation de la forme extrudée autour de l'axe y en degrés.

```csharp
public double RotationY { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Accéder au ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur actuelle de RotationY
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Définir de nouvelles valeurs de RotationY et démontrer les effets
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Appliquer d'autres propriétés 3D pour rendre l'effet visible
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Enregistrer le classeur pour montrer les effets
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Modifier à nouveau la rotation et enregistrer une autre version
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


