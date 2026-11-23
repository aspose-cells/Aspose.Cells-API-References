---
title: "Enum GradientColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.GradientColorType enum. Représente le type de couleur de dégradé pour le remplissage spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Représente le type de couleur de dégradé pour le remplissage spécifié.

```csharp
public enum GradientColorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de couleur de dégradé |
| OneColor | `1` | Une couleur de dégradé |
| PresetColors | `2` | Couleurs de dégradé prédéfinies |
| TwoColors | `3` | Deux couleurs de dégradé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme pour démontrer le remplissage en dégradé
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Définir le type de remplissage en dégradé
                fill.FillType = FillType.Gradient;

                // Démontrer les différentes valeurs de l'énumération GradientColorType
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Lire et afficher le type de couleur de dégradé actuel (la propriété est en lecture seule)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Enregistrez le classeur
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


