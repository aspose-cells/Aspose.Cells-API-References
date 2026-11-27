---
title: "Enum EquationCombiningCharacterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType enum. Typ av kombinerande tecken"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Typ av kombinerande tecken.

```csharp
public enum EquationCombiningCharacterType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Unknown | `-1` | Använd okänd typ när den inte hittas i befintlig typ. |
| DotAbove | `0` | "̇" Unicode: u0307 Kombinerande punkt ovan |
| Diaeresis | `1` | "̈" Unicode: u0308 Kombinerande dieresis |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Kombinerande tre punkter ovan |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Kombinerande cirkumflexaccent |
| Caron | `4` | "̌" Unicode: u030c Kombinerande caron |
| AcuteAccent | `5` | "́" Unicode: u0301 Kombinerande akut accent |
| GraveAccent | `6` | "̀" Unicode: u0300 Kombinerande grav accent |
| Breve | `7` | "̆" Unicode: u0306 Kombinerande kombinerande breve |
| Tilde | `8` | "̃" Unicode: u0303 Kombinerande tilde |
| Overline | `9` | "̅" Unicode: u0305 Kombinerande överlinje |
| DoubleOverline | `10` | "̿" Unicode: u033f Kombinerande dubbel överlinje |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Kombinerande övre krullparentes |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Kombinerande nedre krullparentes |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Kombinerande vänsterpil ovan |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Kombinerande högerpil ovan |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Kombinerande vänster-högerpil ovan |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Kombinerande vänsterhakspets ovan |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Kombinerande högerrakspets ovan |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Vänsterpil |
| RightwardsArrow | `19` | "→" Unicode: u2192 Högerpil |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Vänster-högerpil |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Dubbel vänsterpil |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Dubbel högerpil |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Dubbel vänster-högerpil |

### Exempel

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

            // Verifiera den sparade filen
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

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


