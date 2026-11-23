---
title: "EquationNode.CreateNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Crée un nœud du type spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Créer un nœud du type spécifié.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types de nœuds d'équation |
| classeur | Classeur | L'objet classeur associé à l'équation |
| parent | EquationNode | Le nœud parent où ce nœud est situé |

### Valeur de retour

Si le type spécifié existe, le nœud correspondant est renvoyé, et si le type n'existe pas, un nœud de type inconnu est renvoyé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme d'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Créer un nœud parent (fraction)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Créer les nœuds numérateur et dénominateur
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Ajouter la fraction créée à l'équation principale
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Afficher l'équation dans une cellule
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


