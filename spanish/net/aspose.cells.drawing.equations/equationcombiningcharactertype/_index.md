---
title: "Enumeración EquationCombiningCharacterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType. Tipo de caracteres combinantes"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Tipo de caracteres combinantes.

```csharp
public enum EquationCombiningCharacterType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Unknown | `-1` | Usar tipo desconocido cuando no se encuentre en el tipo existente. |
| DotAbove | `0` | \"̇\" Unicode: u0307 Punto combinante superior |
| Diaeresis | `1` | \"̈\" Unicode: u0308 Diéresis combinante |
| ThreeDotsAbove | `2` | \"⃛\" Unicode: u20db Tres puntos combinantes superiores |
| CircumflexAccent | `3` | \"̂\" Unicode: u0302 Acento circunflejo combinante |
| Caron | `4` | \"̌\" Unicode: u030c Carón combinante |
| AcuteAccent | `5` | \"́\" Unicode: u0301 Acento agudo combinante |
| GraveAccent | `6` | \"̀\" Unicode: u0300 Acento grave combinante |
| Breve | `7` | \"̆\" Unicode: u0306 Breve combinante |
| Tilde | `8` | \"̃\" Unicode: u0303 Tilde combinante |
| Overline | `9` | \"̅\" Unicode: u0305 Línea superior combinante |
| DoubleOverline | `10` | \"̿\" Unicode: u033f Doble línea superior combinante |
| TopCurlyBracket | `11` | \"⏞\" Unicode: u23de Llave rizada superior combinante |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Combinando Corchete Rizado Inferior |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Combinando Flecha Izquierda Sobre |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Combinando Flecha Derecha Sobre |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Combinando Flecha Izquierda Derecha Sobre |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Combinando Garra Izquierda Sobre |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Combinando Garra Derecha Sobre |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Flecha Hacia la Izquierda |
| RightwardsArrow | `19` | "→" Unicode: u2192 Flecha Hacia la Derecha |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Flecha Izquierda Derecha |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Doble Flecha Hacia la Izquierda |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Doble Flecha Hacia la Derecha |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Doble Flecha Izquierda Derecha |

### Ejemplos

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

            // Verifique el archivo guardado
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

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


