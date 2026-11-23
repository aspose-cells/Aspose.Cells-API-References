---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "NaryEquationNode propriété. un opérateur n-aire. p. ex."
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

un opérateur n-aire, p. \"∑\"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accéder à l'équation et ajouter un nœud d'opérateur n-aire
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Caster en NaryEquationNode pour accéder à NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Afficher le NaryOperatorType actuel (valeur par défaut)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Définir l'opérateur de sommation (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Ajouter la base (opérande) et les limites pour démontrer l'opérateur
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Définir l'opérateur pour qu'il s'agrandisse avec son contenu
            naryEquationNode.NaryGrow = true;

            // Passer à l'opérateur produit (∏) et montrer la différence
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Enregistrez le classeur
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


