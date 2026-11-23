---
title: "BarEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode BarEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux instances BarEquationNode pour la comparaison
            // Remarque : La création réelle de BarEquationNode dépendrait des méthodes de fabrique de l'API
            // Pour la démonstration, nous supposerons que ce sont des instances correctement initialisées
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Comparer node1 avec node2 (devrait être égal)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Comparer node1 avec node3 (ne devrait pas être égal)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Comparer node1 avec null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Comparer node1 avec un type d'objet différent
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Méthode d'assistance pour démontrer l'obtention d'un BarEquationNode
        // Dans une utilisation réelle, vous utiliseriez la méthode API appropriée pour les créer
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Ceci n'est qu'un espace réservé - l'implémentation réelle dépendrait de l'API
            // Par exemple, cela pourrait être créé via un objet parent ou une méthode de fabrique
            return null; // Replace with actual creation code
        }
    }
}
```

### Voir aussi

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


