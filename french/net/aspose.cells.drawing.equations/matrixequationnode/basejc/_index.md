---
title: "MatrixEquationNode.BaseJc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "propriété MatrixEquationNode. Cet attribut spécifie la justification de la matrice. Le texte en dehors de la matrice peut être aligné avec le bas, le haut ou le centre d'une fonction de matrice. Par défaut, la matrice suppose une justification centrée."
type: docs
url: /fr/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Cet attribut spécifie l’alignement de la matrice. Le texte en dehors de la matrice peut être aligné en bas, en haut ou au centre d’une fonction de matrice. Par défaut, la matrice utilise l’alignement centré.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyBaseJcDemo
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

            // Définir les propriétés de la matrice, y compris BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Ajouter le contenu d'une matrice 2x2 (matrice identité)
            for (int row = 0; row < 2; row++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Enregistrez le classeur
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Voir aussi

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


