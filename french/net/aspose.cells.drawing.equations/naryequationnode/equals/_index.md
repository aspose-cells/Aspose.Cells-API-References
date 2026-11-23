---
title: "NaryEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NaryEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/naryequationnode/equals/
---
## NaryEquationNode.Equals method

Déterminer si le nœud d'équation actuel est égal au nœud spécifié

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | Le nœud spécifié |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour contenir l'équation
            var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
            var equation1 = shape1.GetEquationParagraph();
            var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode1 = (NaryEquationNode)naryNode1;
            naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Créer une deuxième forme identique
            var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
            var equation2 = shape2.GetEquationParagraph();
            var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode2 = (NaryEquationNode)naryNode2;
            naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Créer une troisième forme différente
            var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
            var equation3 = shape3.GetEquationParagraph();
            var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode3 = (NaryEquationNode)naryNode3;
            naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            try
            {
                // Comparer les nœuds identiques
                bool result1 = naryEquationNode1.Equals(naryEquationNode2);
                Console.WriteLine($"Comparing identical nodes: {result1}");

                // Comparer les nœuds différents
                bool result2 = naryEquationNode1.Equals(naryEquationNode3);
                Console.WriteLine($"Comparing different nodes: {result2}");

                // Comparer avec null
                bool result3 = naryEquationNode1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");

                // Comparer avec un type d'objet différent
                bool result4 = naryEquationNode1.Equals("string object");
                Console.WriteLine($"Comparing with different type: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


