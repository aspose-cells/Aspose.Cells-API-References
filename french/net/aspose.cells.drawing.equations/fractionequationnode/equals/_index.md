---
title: "FractionEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FractionEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Puisque FractionEquationNode n'a pas de constructeur sans paramètre,
                // nous démontrerons Equals avec des objets qui proviendraient probablement d'ailleurs dans l'API
                // À des fins de démonstration, nous supposerons que nous avons deux instances à comparer
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Comparer les objets en utilisant Equals
                bool areEqual = node1.Equals(node2);

                // Afficher le résultat de la comparaison
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Comparer avec null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Comparer avec lui-même
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Méthode d'aide pour simuler l'obtention d'instances de FractionEquationNode
        // (Dans une utilisation réelle, ceux-ci proviendraient de l'API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Ceci n'est qu'un espace réservé - en réalité vous obtiendriez cela de l'API
            // Par exemple : worksheet.Equations.AddFractionEquationNode() ou similaire
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Voir aussi

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


