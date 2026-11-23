---
title: "Classe GradientStop"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.GradientStop. Représente le point d'arrêt du dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Représente le point d'arrêt du dégradé.

```csharp
public class GradientStop
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Obtient la couleur de ce point d'arrêt du dégradé. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | La position du stop. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme avec remplissage en dégradé
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Créer une couleur pour le stop de dégradé
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Ajouter un stop de dégradé
                gradientFill.GradientStops.Add(0, color, 30);

                // Accéder au stop de dégradé
                GradientStop stop = gradientFill.GradientStops[0];

                // Démontrez la fonctionnalité de base
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Modifier les propriétés
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Enregistrez le classeur
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


