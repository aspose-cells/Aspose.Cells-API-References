---
title: "PatternFill.ForegroundCellsColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PatternFill. Obtient et définit l’objet CellsColor de premier plan"
type: docs
url: /fr/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Obtient et définit l’objet [`CellsColor`](../../../aspose.cells/cellscolor/) de premier plan.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le remplissage par motif
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Définissez le type de remplissage sur motif
                shape.Fill.FillType = FillType.Pattern;

                // Obtenez l’instance de PatternFill
                PatternFill patternFill = shape.Fill.PatternFill;

                // Définissez le type de motif et les couleurs
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Créez un objet CellsColor pour le premier plan en utilisant la propriété Color
                // Comme CellsColor n'a pas de constructeur public, nous utiliserons le ForegroundCellsColor existant
                // et modifiez ses propriétés directement
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Affichez les propriétés du ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Enregistrez le classeur
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


