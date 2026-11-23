---
title: "ThreeDFormat.ExtrusionHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la hauteur d'extrusion appliquée à la forme en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

Obtient et définit la hauteur d'extrusion appliquée à la forme, en unités de points.

```csharp
public double ExtrusionHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyExtrusionHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Appliquer le formatage 3D
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionHeight = 32;
            threeDFormat.ContourWidth = 17;
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifiez les valeurs enregistrées
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


