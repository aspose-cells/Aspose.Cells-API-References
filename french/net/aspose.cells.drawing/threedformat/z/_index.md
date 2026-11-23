---
title: "ThreeDFormat.Z"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Définit la distance du sol pour la forme 3D"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Définit la distance du sol pour la forme 3D.

```csharp
public double Z { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Accéder au ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur actuelle de Z (distance du sol)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Définir une nouvelle valeur de Z pour éloigner la forme du sol
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Configurer d'autres propriétés 3D pour rendre l'effet visible
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Enregistrer le classeur pour voir l'effet 3D
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


