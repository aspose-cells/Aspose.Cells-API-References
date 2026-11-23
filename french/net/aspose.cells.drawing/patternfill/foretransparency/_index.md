---
title: "PatternFill.ForeTransparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PatternFill. Obtient ou définit la transparence de la couleur du premier plan"
type: docs
url: /fr/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Obtient ou définit la transparence de la couleur de premier plan.

```csharp
public double ForeTransparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le remplissage par motif
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Définissez le type de remplissage sur motif
            shape.Fill.FillType = FillType.Pattern;

            // Obtenez l’instance de PatternFill
            PatternFill patternFill = shape.Fill.PatternFill;

            // Configurez les propriétés de remplissage du motif
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Affichez la valeur initiale de ForeTransparency
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Définissez une nouvelle valeur de ForeTransparency (transparence de 50 %)
                patternFill.ForeTransparency = 0.5;

                // Affichez la valeur mise à jour de ForeTransparency
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Enregistrez le classeur
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


