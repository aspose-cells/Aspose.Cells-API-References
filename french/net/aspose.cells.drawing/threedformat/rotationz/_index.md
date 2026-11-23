---
title: "ThreeDFormat.RotationZ"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la rotation de la forme extrudée autour de l'axe z en degrés"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Obtient et définit la rotation de la forme extrudée autour de l'axe z en degrés.

```csharp
public double RotationZ { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Accéder au ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur actuelle de RotationZ
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Définir de nouvelles valeurs de RotationZ et démontrer les effets
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Appliquer d'autres propriétés 3D pour rendre la rotation visible
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Enregistrer le classeur avec les effets 3D
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


