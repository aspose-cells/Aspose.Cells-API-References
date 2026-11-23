---
title: "BoxEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode BoxEquationNode. Déterminez si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez deux objets BoxEquationNode pour la comparaison
            // Étant donné que BoxEquationNode n'a pas de constructeur sans paramètres,
            // nous devrons les créer différemment. En supposant que nous puissions les obtenir de quelque part,
            // ou les créer avec certains paramètres par défaut.
            // À des fins de démonstration, nous les déclarerons simplement et assignerons null (bien que dans le code réel vous ayez besoin d'une initialisation appropriée)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Appelez la méthode Equals avec les types de paramètres spécifiques (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // Afficher le résultat
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Ajouter le résultat à la feuille de calcul
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Enregistrer le résultat
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


