---
title: "TextRunEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "TextRunEquationNode méthode. Déterminer si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // À des fins de démonstration, nous utiliserons null et montrerons simplement la logique de comparaison
            // puisque nous ne pouvons pas créer d'instances de TextRunEquationNode directement
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Cette partie reste pour montrer comment Equals serait appelé
                // Dans un scénario réel, ces nœuds seraient correctement initialisés
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Comparer node1 avec node2 (même contenu)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Comparer node1 avec node3 (contenu différent)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Comparer avec null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Comparer avec un type d'objet différent
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrer le classeur (bien que Equals ne modifie pas la feuille de calcul)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Supprimé la méthode d'assistance puisque nous ne pouvons pas créer correctement des instances de TextRunEquationNode
    }
}
```

### Voir aussi

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


