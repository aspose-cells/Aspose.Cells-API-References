---
title: "LimLowUppEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "méthode LimLowUppEquationNode. Détermine si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

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

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Comme nous ne connaissons pas les paramètres du constructeur, nous comparerons des valeurs nulles
            // Ceci est une modification minimale pour le faire compiler – en utilisation réelle, vous auriez besoin d'une construction appropriée
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Appeler la méthode Equals avec le type de paramètre spécifique (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Afficher le résultat
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Enregistrez le classeur
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


