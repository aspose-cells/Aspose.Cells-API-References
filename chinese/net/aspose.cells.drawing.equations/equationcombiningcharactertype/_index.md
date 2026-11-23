---
title: "枚举 EquationCombiningCharacterType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType 枚举。组合字符的类型"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

组合字符的类型。

```csharp
public enum EquationCombiningCharacterType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Unknown | `-1` | 在现有类型中未找到时使用 unknown 类型。 |
| DotAbove | `0` | "̇" Unicode: u0307 组合上点 |
| Diaeresis | `1` | "̈" Unicode: u0308 组合分音符 |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db 组合上方三点 |
| CircumflexAccent | `3` | "̂" Unicode: u0302 组合抑扬符 |
| Caron | `4` | "̌" Unicode: u030c 组合抑扬符 |
| AcuteAccent | `5` | "́" Unicode: u0301 组合锐音符 |
| GraveAccent | `6` | "̀" Unicode: u0300 组合抑音符 |
| Breve | `7` | "̆" Unicode: u0306 组合短音符 |
| Tilde | `8` | "̃" Unicode: u0303 组合波浪号 |
| Overline | `9` | "̅" Unicode: u0305 组合上划线 |
| DoubleOverline | `10` | "̿" Unicode: u033f 组合双上划线 |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de 组合上花括号 |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df 组合下花括号 |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 组合上方左箭头 |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 组合上方右箭头 |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 组合上方左右箭头 |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 组合上方左叉 |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 组合上方右叉 |
| LeftwardsArrow | `18` | "←" Unicode: u2190 左向箭头 |
| RightwardsArrow | `19` | "→" Unicode: u2192 右向箭头 |
| LeftRightArrow | `20` | "↔" Unicode: u2194 左右箭头 |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 左向双箭头 |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 右向双箭头 |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 左右双箭头 |

### 示例

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

            // 验证已保存的文件
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

### 另请参见

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


