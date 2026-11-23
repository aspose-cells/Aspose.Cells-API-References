---
title: "DelimiterEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DelimiterEquationNode. Déterminer si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/delimiterequationnode/equals/
---
## DelimiterEquationNode.Equals method

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

    public class DelimiterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux instances de DelimiterEquationNode pour la comparaison
            // Puisque DelimiterEquationNode n'a pas de constructeur sans paramètre,
            // nous devrons les créer différemment. En supposant que nous puissions utiliser le constructeur par défaut
            // de la classe de base ou trouver une autre façon de les créer.
            // Pour la démonstration, nous utiliserons ObjectCreationHelper (hypothétique) ou une approche similaire
            DelimiterEquationNode node1 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node1.BeginChar = "(";
            node1.EndChar = ")";
            node1.SeparatorChar = ",";
            node1.DelimiterShape = EquationDelimiterShapeType.Centered;

            DelimiterEquationNode node2 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node2.BeginChar = "(";
            node2.EndChar = ")";
            node2.SeparatorChar = ",";
            node2.DelimiterShape = EquationDelimiterShapeType.Centered;

            try
            {
                // Appelez la méthode Equals avec le paramètre Object
                bool result = node1.Equals((Object)node2);

                // Afficher le résultat
                Console.WriteLine($"Equals method result: {result}");

                // Modifier node2 pour les rendre différents
                node2.BeginChar = "[";
                bool result2 = node1.Equals((Object)node2);
                Console.WriteLine($"Equals method result after modification: {result2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


