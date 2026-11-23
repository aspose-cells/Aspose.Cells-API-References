---
title: "Énumération EquationVerticalJustificationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType enum. Cela spécifie l'alignement vertical par défaut des équations dans le document"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationverticaljustificationtype/
---
## EquationVerticalJustificationType enumeration

Cela spécifie l'alignement vertical par défaut des équations dans le document.

```csharp
public enum EquationVerticalJustificationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Top | `0` | haut |
| Center | `1` | centre |
| Bottom | `2` | bas |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationVerticalJustificationTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le paragraphe d’équation et ajouter un nœud de matrice
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Définir les propriétés de la matrice
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Ajouter des lignes et des colonnes de matrice
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Enregistrez le classeur
            string outputPath = "EquationVerticalJustificationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("File saved with vertical justification demo: " + outputPath);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


