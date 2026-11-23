---
title: "EquationNode.RemoveAllChildren"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Supprime tous les nœuds enfants du nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/removeallchildren/
---
## EquationNode.RemoveAllChildren method

Supprime tous les nœuds enfants du nœud actuel.

```csharp
public void RemoveAllChildren()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveAllChildrenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Obtenir le nœud d'équation
            var equationNode = ((TextBox)shape).GetEquationParagraph();

            // Ajouter quelques nœuds enfants à l'équation
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML

            Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");

            try
            {
                // Appeler la méthode RemoveAllChildren
                equationNode.RemoveAllChildren();

                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


