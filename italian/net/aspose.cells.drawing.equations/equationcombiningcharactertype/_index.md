---
title: "Enum EquationCombiningCharacterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType enum. Tipo di caratteri combinanti"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Tipo di caratteri combinanti.

```csharp
public enum EquationCombiningCharacterType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Unknown | `-1` | Usa il tipo sconosciuto quando non viene trovato nel tipo esistente. |
| DotAbove | `0` | "̇" Unicode: u0307 Punto combinante sopra |
| Diaeresis | `1` | "̈" Unicode: u0308 Diaeresi combinante |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Tre punti combinanti sopra |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Accento circonflesso combinante |
| Caron | `4` | "̌" Unicode: u030c Caron combinante |
| AcuteAccent | `5` | "́" Unicode: u0301 Accento acuto combinante |
| GraveAccent | `6` | "̀" Unicode: u0300 Accento grave combinante |
| Breve | `7` | "̆" Unicode: u0306 Breve combinante |
| Tilde | `8` | "̃" Unicode: u0303 Tilde combinante |
| Overline | `9` | "̅" Unicode: u0305 Linea sopra combinante |
| DoubleOverline | `10` | "̿" Unicode: u033f Doppia linea sopra combinante |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Graffa curva superiore combinante |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Parentesi graffa inferiore combinata |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Freccia sinistra combinata sopra |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Freccia destra combinata sopra |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Freccia sinistra-destra combinata sopra |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Arpione sinistro combinato sopra |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Arpione destro combinato sopra |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Freccia verso sinistra |
| RightwardsArrow | `19` | "→" Unicode: u2192 Freccia verso destra |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Freccia sinistra-destra |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Doppia freccia verso sinistra |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Doppia freccia verso destra |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Doppia freccia sinistra-destra |

### Esempi

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

            // Verifica il file salvato
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

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


