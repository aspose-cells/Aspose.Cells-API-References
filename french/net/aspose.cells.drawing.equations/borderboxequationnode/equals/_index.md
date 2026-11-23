---
title: "BorderBoxEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode BorderBoxEquationNode. Déterminer si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Créer deux instances de BorderBoxEquationNode pour la comparaison
                // Comme BorderBoxEquationNode n'a pas de constructeur sans paramètres,
                // nous utiliserons le constructeur de la classe de base (en supposant qu'EquationNode en possède un)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Comparer les nœuds en utilisant la méthode Equals
                bool areEqual = node1.Equals((object)node2);
                
                // Afficher le résultat de la comparaison
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Comparer avec un type d'objet différent
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


