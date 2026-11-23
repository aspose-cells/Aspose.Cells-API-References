---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "propriété MatrixEquationNode. Cet attribut spécifie la propriété Masquer les espaces réservés sur une matrice. Lorsque cette propriété est activée, les espaces réservés n'apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent afin que les emplacements où du texte peut être inséré soient visibles."
type: docs
url: /fr/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Cet attribut spécifie la propriété Masquer les espaces réservés sur une matrice. Lorsque cette propriété est activée, les espaces réservés n’apparaissent pas dans la matrice. Par défaut, les espaces réservés apparaissent afin que les emplacements où le texte peut être inséré soient visibles.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'équation
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud mathématique et ajouter la matrice
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Définir les propriétés de la matrice
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Ajouter une matrice 2x2 avec des 1 sur la diagonale
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Enregistrer et vérifier
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


