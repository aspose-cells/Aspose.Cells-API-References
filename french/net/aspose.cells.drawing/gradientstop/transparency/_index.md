---
title: "GradientStop.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientStop. Renvoie ou définit le degré de transparence de la zone sous forme d'une valeur de 0.0 opaque à 1.0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme avec remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Créer une couleur pour le stop de dégradé
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Ajouter un arrêt de dégradé avec une transparence initiale
            gradientFill.GradientStops.Add(0, color, 30);

            // Accéder au stop de dégradé
            GradientStop stop = gradientFill.GradientStops[0];

            // Afficher et modifier la transparence
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Ajouter un autre arrêt pour une comparaison visuelle
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Enregistrez le classeur
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


