---
title: "ThreeDFormat.RotationX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la rotation de la forme extrudée autour de l'axe x en degrés"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Obtient et définit la rotation de la forme extrudée autour de l'axe x en degrés.

```csharp
public double RotationX { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // Obtenir le format 3D (pas besoin de "activer" les effets 3D - il suffit de définir les propriétés)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur actuelle de RotationX
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Définir une nouvelle valeur de RotationX (rotation autour de l'axe x en degrés)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Définir d'autres propriétés 3D pour rendre la rotation visible
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Enregistrer le classeur pour voir les effets
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


