---
title: "Enum EquationCombiningCharacterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType enum. Birleştirici karakterlerin türü"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Birleştirici karakterlerin türü.

```csharp
public enum EquationCombiningCharacterType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Unknown | `-1` | Mevcut türde bulunmadığında bilinmeyen türü kullan. |
| DotAbove | `0` | "̇" Unicode: u0307 Üstte Birleştirilen Nokta |
| Diaeresis | `1` | "̈" Unicode: u0308 Üstte Birleştirilen İki Nokta |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Üstte Birleştirilen Üç Nokta |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Üstte Birleştirilen Şapka İşareti |
| Caron | `4` | "̌" Unicode: u030c Üstte Birleştirilen Caron |
| AcuteAccent | `5` | "́" Unicode: u0301 Üstte Birleştirilen Keskin Aksan |
| GraveAccent | `6` | "̀" Unicode: u0300 Üstte Birleştirilen Grave Aksan |
| Breve | `7` | "̆" Unicode: u0306 Üstte Birleştirilen Breve |
| Tilde | `8` | "̃" Unicode: u0303 Üstte Birleştirilen Tilde |
| Overline | `9` | "̅" Unicode: u0305 Üstte Birleştirilen Üst Çizgi |
| DoubleOverline | `10` | "̿" Unicode: u033f Üstte Birleştirilen Çift Üst Çizgi |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Üstte Birleştirilen Üst Kıvrımlı Parantez |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Alt Kıvrımlı Parantez |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Üstünde Sol Ok |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Üstünde Sağ Ok |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Üstünde Sol Sağ Ok |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Üstünde Sol Kanca |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Üstünde Sağ Kanca |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Sol Yönlü Ok |
| RightwardsArrow | `19` | "→" Unicode: u2192 Sağ Yönlü Ok |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Sol Sağ Ok |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Sol Yönlü Çift Ok |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Sağ Yönlü Çift Ok |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Sol Sağ Çift Ok |

### Örnekler

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

            // Kaydedilen dosyayı doğrula
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


