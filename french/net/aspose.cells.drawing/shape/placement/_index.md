---
title: "Shape.Placement"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

```csharp
public PlacementType Placement { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Démontrer la propriété Placement
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Modifiez le type de placement
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Enregistrez le classeur
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


