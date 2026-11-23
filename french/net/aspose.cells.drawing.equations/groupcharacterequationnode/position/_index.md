---
title: "GroupCharacterEquationNode.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GroupCharacterEquationNode. Cet attribut spécifie la position du caractère dans l'objet"
type: docs
url: /fr/net/aspose.cells.drawing.equations/groupcharacterequationnode/position/
---
## GroupCharacterEquationNode.Position property

Cet attribut spécifie la position du caractère dans l'objet

```csharp
public EquationCharacterPositionType Position { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une forme d'équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le paragraphe d'équation et ajouter un nœud de caractère de groupe
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Définir la propriété de position (démonstration principale)
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Ajouter le texte de base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";

            // Enregistrez le classeur
            string outputPath = "GroupCharacterEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Equation with group character position set to Top has been created successfully.");
        }
    }
}
```

### Voir aussi

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


