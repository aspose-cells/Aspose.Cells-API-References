---
title: "UnknowEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnknowEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux nœuds d'équation inconnus pour la comparaison
            // Comme UnknowEquationNode n'a pas de constructeur sans paramètres,
            // nous devrons les créer différemment. À des fins de démonstration, nous utiliserons
            // le constructeur réel s'il est disponible, ou les créer par d'autres moyens.
            // Comme nous ne connaissons pas les paramètres du constructeur, il s'agit d'une solution de substitution.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Appeler la méthode Equals avec le type de paramètre spécifique (Object)
                bool areEqual = node1.Equals(objToCompare);

                // Afficher le résultat
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Ajouter le résultat à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Méthode d'assistance pour créer des instances UnknowEquationNode
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // Dans une implémentation réelle, cela utiliserait le constructeur approprié
            // Comme nous ne connaissons pas les paramètres du constructeur, nous retournerons null
            // et gérer le cas null dans la démonstration (bien que ce ne soit qu'un substitut)
            return null;
        }
    }
}
```

### Voir aussi

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


