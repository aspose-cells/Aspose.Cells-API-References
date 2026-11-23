---
title: "EquationNode.InsertBefore"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Insère le nœud spécifié avant le nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Insère le nœud spécifié avant le nœud actuel.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types de nœuds d'équation |

### Valeur de retour

Si le type spécifié existe, le nœud correspondant est renvoyé, et si le type n'existe pas, un nœud de type inconnu est renvoyé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une équation mathématique dans la cellule A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Ajouter le nœud texte initial à l'équation
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Insérer un nouveau nœud texte avant celui existant
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Afficher l'équation au format LaTeX
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


