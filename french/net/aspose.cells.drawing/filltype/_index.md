---
title: "Enum FillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.FillType enum. Type de format de remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Type de format de remplissage.

```csharp
public enum FillType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Représente le type de formatage automatique. |
| None | `1` | Représente le type de formatage aucun. |
| Solid | `2` | Format de remplissage solide. |
| Gradient | `3` | Format de remplissage en dégradé. |
| Texture | `4` | Format de remplissage texture(inclut le remplissage d'image). |
| Pattern | `5` | Format de remplissage en motif. |
| Group | `6` | Hériter des propriétés de remplissage du groupe. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Définir le type de remplissage en dégradé
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Ajouter une zone de texte
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Définir le type de remplissage en dégradé pour la zone de texte
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Enregistrez le classeur
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


