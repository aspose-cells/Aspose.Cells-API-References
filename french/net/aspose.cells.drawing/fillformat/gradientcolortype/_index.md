---
title: "FillFormat.GradientColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Retourne le type de couleur de dégradé pour le remplissage spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Renvoie le type de couleur de dégradé pour le remplissage spécifié.

```csharp
public GradientColorType GradientColorType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Définir un remplissage en dégradé à deux couleurs
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Accédez à FillFormat pour obtenir GradientColorType
                FillFormat fillFormat = shape.Fill;

                // Afficher la valeur de GradientColorType
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Enregistrez le classeur
                workbook.Save("GradientColorTypeDemo.xlsx");
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

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


