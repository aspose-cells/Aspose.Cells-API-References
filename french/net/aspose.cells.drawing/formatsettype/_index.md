---
title: "Enum FormatSetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.FormatSetType enum. Type de jeu de format de remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Type d'ensemble de format de remplissage.

```csharp
public enum FormatSetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun format de remplissage. |
| IsGradientSet | `1` | Format de remplissage en dégradé. |
| IsTextureSet | `2` | Format de remplissage en texture. |
| IsPatternSet | `3` | Format de remplissage en motif. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajoutez une forme pour démontrer le format de remplissage
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Afficher le type de remplissage initial
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Démontrer les valeurs de l'énumération FormatSetType
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Appliquer différents types de remplissage en utilisant FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Enregistrez le classeur
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


