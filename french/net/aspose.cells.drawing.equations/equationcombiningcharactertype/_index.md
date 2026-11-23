---
title: "Énumération EquationCombiningCharacterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType. Type de caractères combinés"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Type de caractères combinés.

```csharp
public enum EquationCombiningCharacterType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Unknown | `-1` | Utilisez le type inconnu lorsqu'il n'est pas trouvé dans le type existant. |
| DotAbove | `0` | "̇" Unicode : u0307 Point combiné au-dessus |
| Diaeresis | `1` | "̈" Unicode : u0308 Tréma combiné |
| ThreeDotsAbove | `2` | "⃛" Unicode : u20db Trois points combinés au-dessus |
| CircumflexAccent | `3` | "̂" Unicode : u0302 Accent circonflexe combiné |
| Caron | `4` | "̌" Unicode : u030c Caron combiné |
| AcuteAccent | `5` | "́" Unicode : u0301 Accent aigu combiné |
| GraveAccent | `6` | "̀" Unicode : u0300 Accent grave combiné |
| Breve | `7` | "̆" Unicode : u0306 Brève combinée |
| Tilde | `8` | "̃" Unicode : u0303 Tilde combiné |
| Overline | `9` | "̅" Unicode : u0305 Ligne supérieure combinée |
| DoubleOverline | `10` | "̿" Unicode : u033f Double ligne supérieure combinée |
| TopCurlyBracket | `11` | "⏞" Unicode : u23de Accolade supérieure courbée combinée |
| BottomCurlyBracket | `12` | "⏟" Unicode : u23df Accolade incurvée inférieure combinée |
| LeftArrowAbove | `13` | "⃖" Unicode : u20d6 Flèche gauche combinée au-dessus |
| RightArrowAbove | `14` | "⃗" Unicode : u20d7 Flèche droite combinée au-dessus |
| LeftRightArrowAbove | `15` | "⃡" Unicode : u20e1 Flèche gauche-droite combinée au-dessus |
| LeftHarpoonAbove | `16` | "⃐" Unicode : u20d0 Harpon gauche combiné au-dessus |
| RightHarpoonAbove | `17` | "⃑" Unicode : u20d1 Harpon droit combiné au-dessus |
| LeftwardsArrow | `18` | "←" Unicode : u2190 Flèche vers la gauche |
| RightwardsArrow | `19` | "→" Unicode : u2192 Flèche vers la droite |
| LeftRightArrow | `20` | "↔" Unicode : u2194 Flèche gauche-droite |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode : u21d0 Double flèche vers la gauche |
| RightwardsDoubleArrow | `22` | "⇒" Unicode : u21d2 Double flèche vers la droite |
| LeftRightDoubleArrow | `23` | "⇔" Unicode : u21d4 Double flèche gauche-droite |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCombiningCharacterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            node.Position = EquationCharacterPositionType.Top;
            node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode textRun = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            textRun.Text = "abc";

            string resultFile = "GroupCharacterEquationTest.xlsx";
            workbook.Save(resultFile);

            // Vérifier le fichier enregistré
            Workbook workbook2 = new Workbook(resultFile);
            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node2 = (GroupCharacterEquationNode)mathNode2.GetChild(0);

            Console.WriteLine("Equation Type: " + node2.EquationType);
            Console.WriteLine("Position: " + node2.Position);
            Console.WriteLine("Character Type: " + node2.ChrType);
            Console.WriteLine("Group Character: " + node2.GroupChr);

            EquationNode baseNode = node2.GetChild(0);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.GetChild(0);
            Console.WriteLine("Text Content: " + textNode.Text);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


