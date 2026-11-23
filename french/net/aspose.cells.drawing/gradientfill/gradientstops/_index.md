---
title: "GradientFill.GradientStops"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientFill. Représente la collection de points d'arrêt du dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Représente la collection de points d'arrêt du dégradé.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyGradientStopsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            
            // Ajouter une forme rectangulaire
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Définir le remplissage en dégradé
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Effacer tous les points d'arrêt de dégradé existants
            gradientFill.GradientStops.Clear();

            // Ajouter des points d'arrêt de dégradé personnalisés
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Démontrer l'accès aux points d'arrêt du dégradé
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


