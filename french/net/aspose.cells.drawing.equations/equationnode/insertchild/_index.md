---
title: "EquationNode.InsertChild"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode EquationNode. Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Insère un nœud du type spécifié à la position d'index spécifiée dans la liste des nœuds enfants du nœud actuel.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | valeur d'index |
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

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme d'équation
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Ajouter le nœud texte initial à l'équation
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Insérer un nouveau nœud fraction à l'index 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Enregistrez le classeur
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


