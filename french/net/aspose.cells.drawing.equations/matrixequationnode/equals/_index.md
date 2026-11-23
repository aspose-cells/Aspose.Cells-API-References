---
title: "MatrixEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "méthode MatrixEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/matrixequationnode/equals/
---
## MatrixEquationNode.Equals method

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

    public class MatrixEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Comme MatrixEquationNode n'a pas de constructeur sans paramètres,
                // nous démontrerons la méthode Equals en utilisant une approche différente
                Console.WriteLine("MatrixEquationNode Equals demonstration:");
                
                // Remarque : L'instanciation réelle nécessiterait des paramètres de constructeur appropriés
                // Ceci n'est qu'une démonstration du modèle d'utilisation de la méthode Equals
                MatrixEquationNode node1 = null; // Would normally be created with proper constructor
                MatrixEquationNode node2 = null; // Would normally be created with proper constructor

                if (node1 != null && node2 != null)
                {
                    // Comparer les nœuds en utilisant la méthode Equals
                    bool areEqual = node1.Equals(node2);
                    Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");

                    // Comparer un nœud avec lui-même
                    bool selfEqual = node1.Equals(node1);
                    Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
                }

                // Comparer avec null
                if (node1 != null)
                {
                    bool nullEqual = node1.Equals(null);
                    Console.WriteLine($"Is node1 equal to null? {nullEqual}");
                }
                else
                {
                    Console.WriteLine("Node1 is null - cannot demonstrate Equals method");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MatrixEquationNode Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


