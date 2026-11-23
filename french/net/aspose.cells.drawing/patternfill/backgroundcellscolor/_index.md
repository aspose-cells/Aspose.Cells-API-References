---
title: "PatternFill.BackgroundCellsColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PatternFill. Obtient et définit l’objet CellsColor de premier plan"
type: docs
url: /fr/net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

Obtient et définit l’objet [`CellsColor`](../../../aspose.cells/cellscolor/) de premier plan.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackgroundCellsColorDemo
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

                // Accédez et modifiez les propriétés de BackgroundCellsColor
                patternFill.BackgroundCellsColor.Color = Color.Blue;
                patternFill.BackgroundCellsColor.Argb = Color.Blue.ToArgb();
                patternFill.BackgroundCellsColor.Transparency = 0.3;

                // Affichez les propriétés du BackgroundCellsColor
                Console.WriteLine("BackgroundCellsColor Type: " + patternFill.BackgroundCellsColor.Type);
                Console.WriteLine("BackgroundCellsColor Color: " + patternFill.BackgroundCellsColor.Color);
                Console.WriteLine("BackgroundCellsColor ARGB: " + patternFill.BackgroundCellsColor.Argb);
                Console.WriteLine("BackgroundCellsColor Transparency: " + patternFill.BackgroundCellsColor.Transparency);

                // Enregistrez le classeur
                workbook.Save("BackgroundCellsColorDemo.xlsx");
                Console.WriteLine("BackgroundCellsColor demonstration completed successfully.");
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


