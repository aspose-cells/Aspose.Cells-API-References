---
title: "GroupCharacterEquationNode.ChrType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GroupCharacterEquationNode. Spécifier les caractères combinés par valeur de type"
type: docs
url: /fr/net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Spécifier les caractères combinés par valeur de type.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyChrTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud racine de l'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Ajouter un nœud de caractère de groupe
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Définir les propriétés du caractère de groupe
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Ajouter le texte de base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "test";

            // Enregistrez le classeur
            workbook.Save("GroupCharacterEquationDemo.xlsx");

            // Vérifier le fichier enregistré
            Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);

            Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
            Console.WriteLine("Group Character: " + verifyNode.GroupChr);
            Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Voir aussi

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


