---
title: "ThreeDFormat.Perspective"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit l'angle sous lequel un objet ThreeDFormat peut être visualisé"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Obtient et définit l'angle sous lequel un objet ThreeDFormat peut être visualisé.

```csharp
public double Perspective { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Obtenez le format 3D de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Affichez la valeur actuelle de la perspective
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Définissez une nouvelle valeur de perspective (0 à 120 degrés)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Appliquez d'autres effets 3D pour mieux visualiser le changement de perspective
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Enregistrer le classeur pour voir les effets
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


