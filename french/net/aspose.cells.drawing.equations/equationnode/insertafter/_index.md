---
title: "EquationNode.InsertAfter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Insère le nœud spécifié après le nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Insère le nœud spécifié après le nœud actuel.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme d'équation dans la cellule A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Ajouter le nœud texte initial
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Insérer un nouveau nœud texte après celui existant
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Afficher la structure de l'équation
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Enregistrer l'équation dans une cellule pour une inspection visuelle
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


