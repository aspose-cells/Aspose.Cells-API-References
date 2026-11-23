---
title: "GradientStop.CellsColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientStop. Obtient la couleur de cet arrêt de dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Obtient la couleur de ce point d'arrêt du dégradé.

```csharp
public CellsColor CellsColor { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
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

                // Accéder à l'arrêt de dégradé et afficher ses propriétés CellsColor
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Enregistrez le classeur
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


