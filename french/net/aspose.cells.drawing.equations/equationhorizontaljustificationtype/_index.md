---
title: "Énumération EquationHorizontalJustificationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. Cela spécifie la justification horizontale par défaut des équations dans le document"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

Cela spécifie l'alignement horizontal par défaut des équations dans le document.

```csharp
public enum EquationHorizontalJustificationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Center | `0` | Centré |
| CenterGroup | `1` | Centré en groupe |
| Left | `2` | Justifié à gauche |
| Right | `3` | Aligné à droite |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme d'équation à la feuille de calcul
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Obtenir le paragraphe d'équation
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // Démontrer différents types de justification horizontale
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // Enregistrez le classeur
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


