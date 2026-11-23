---
title: "MathematicalEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode MathematicalEquationNode. Déterminez si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Créez deux instances de MathematicalEquationNode pour la comparaison
                // Étant donné que MathematicalEquationNode n'a pas de constructeur sans paramètres,
                // nous devrons passer null ou des paramètres appropriés
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Comparer les nœuds en utilisant la méthode Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Afficher le résultat de la comparaison
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Comparer avec un type d'objet différent
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


