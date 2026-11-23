---
title: "FunctionEquationNode.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FunctionEquationNode. Déterminer si le nœud d'équation actuel est égal au nœud spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Déterminer si le nœud d'équation actuel est égal au nœud spécifié

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | Le nœud spécifié |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme TextBox pour contenir une équation
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Obtenir le nœud d'équation racine du TextBox
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer le premier nœud d'équation fonction
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Optionnel) Ajouter un contenu minimal pour rendre le nœud valide
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Créer le deuxième nœud d'équation fonction
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Comparer les deux nœuds fonction en utilisant Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Comparer un nœud à lui-même
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Enregistrer le classeur (aucun changement visuel nécessaire pour cette démonstration)
                workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


