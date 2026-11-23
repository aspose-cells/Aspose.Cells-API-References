---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GroupCharacterEquationNode. Spécifie un symbole par défaut U23DF. Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu"
type: docs
url: /fr/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Spécifie un symbole (par défaut U+23DF). Il est fortement recommandé d'utiliser l'attribut ChrType pour définir le caractère d'accent. Utilisez ce paramètre de propriété si vous ne trouvez pas le caractère dont vous avez besoin dans un type connu.

```csharp
public string GroupChr { get; set; }
```

### Remarques

Il convient de noter que cette propriété n'accepte qu'un seul caractère, et si plusieurs caractères sont fournis, seul le premier caractère est accepté.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une équation à la première feuille de calcul
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Obtenir le nœud racine de l'équation
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Créer un nœud de caractère de groupe avec une double flèche vers la droite
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Ajouter le texte de base au caractère de groupe
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Démontrer l'utilisation de la propriété GroupChr
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Enregistrez le classeur
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


