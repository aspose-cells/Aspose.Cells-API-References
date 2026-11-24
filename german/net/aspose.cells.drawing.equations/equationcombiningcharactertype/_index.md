---
title: "Enum EquationCombiningCharacterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType Enum. Typ der kombinierenden Zeichen"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Typ von Kombinationszeichen.

```csharp
public enum EquationCombiningCharacterType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Unknown | `-1` | Verwenden Sie den unbekannten Typ, wenn er im vorhandenen Typ nicht gefunden wird. |
| DotAbove | `0` | "̇" Unicode: u0307 Kombinierender Punkt darüber |
| Diaeresis | `1` | "̈" Unicode: u0308 Kombinierender Umlaut |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Kombinierende drei Punkte darüber |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Kombinierender Zirkumflexakzent |
| Caron | `4` | "̌" Unicode: u030c Kombinierender Caron |
| AcuteAccent | `5` | "́" Unicode: u0301 Kombinierender Akutakzent |
| GraveAccent | `6` | "̀" Unicode: u0300 Kombinierender Gravisakzent |
| Breve | `7` | "̆" Unicode: u0306 Kombinierendes Breve |
| Tilde | `8` | "̃" Unicode: u0303 Kombinierende Tilde |
| Overline | `9` | "̅" Unicode: u0305 Kombinierende Oberlinie |
| DoubleOverline | `10` | "̿" Unicode: u033f Kombinierende doppelte Oberlinie |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Kombinierende obere geschwungene Klammer |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Kombinierende untere geschwungene Klammer |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Kombinierender Pfeil nach links darüber |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Kombinierender Pfeil nach rechts darüber |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Kombinierender Pfeil nach links/rechts darüber |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Kombinierender linker Haken darüber |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Kombinierender rechter Haken darüber |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Linkspfeil |
| RightwardsArrow | `19` | "→" Unicode: u2192 Rechtspfeil |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Links‑Rechts‑Pfeil |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Doppelter Linkspfeil |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Doppelter Rechtspfeil |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Links Rechts Doppelpfeil |

### Beispiele

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

            // Überprüfen Sie die gespeicherte Datei
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

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


