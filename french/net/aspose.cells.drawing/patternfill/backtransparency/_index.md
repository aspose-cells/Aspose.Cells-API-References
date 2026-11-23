---
title: "PatternFill.BackTransparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PatternFill. Obtient ou définit la transparence de la couleur d'arrière-plan"
type: docs
url: /fr/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Obtient ou définit la transparence de la couleur d'arrière-plan.

```csharp
public double BackTransparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Obtenez l'instance PatternFill existante à partir de la forme et configurez ses propriétés
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Affichez la valeur initiale de BackTransparency
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Définissez une nouvelle valeur de BackTransparency (transparence de 50 %)
            patternFill.BackTransparency = 0.5;

            // Enregistrer le classeur modifié
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


