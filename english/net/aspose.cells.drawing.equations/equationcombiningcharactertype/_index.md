---
title: Enum EquationCombiningCharacterType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType enum. Type of combining characters
type: docs
url: /net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

Type of combining characters.

```csharp
public enum EquationCombiningCharacterType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Unknown | `-1` | Use unknown type when not found in existing type. |
| DotAbove | `0` | "̇" Unicode: u0307 Combining Dot Above |
| Diaeresis | `1` | "̈" Unicode: u0308 Combining Diaeresis |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db Combining Three Dots Above |
| CircumflexAccent | `3` | "̂" Unicode: u0302 Combining Circumflex Accent |
| Caron | `4` | "̌" Unicode: u030c Combining Caron |
| AcuteAccent | `5` | "́" Unicode: u0301 Combining Acute Accent |
| GraveAccent | `6` | "̀" Unicode: u0300 Combining Grave Accent |
| Breve | `7` | "̆" Unicode: u0306 Combining Combining Breve |
| Tilde | `8` | "̃" Unicode: u0303 Combining Tilde |
| Overline | `9` | "̅" Unicode: u0305 Combining Overline |
| DoubleOverline | `10` | "̿" Unicode: u033f Combining Double Overline |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de Combining Top Curly Bracket |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df Combining Bottom Curly Bracket |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 Combining Left Arrow Above |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 Combining Right Arrow Above |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 Combining Left Right Arrow Above |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 Combining Left Harpoon Above |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 Combining Right Harpoon Above |
| LeftwardsArrow | `18` | "←" Unicode: u2190 Leftwards Arrow |
| RightwardsArrow | `19` | "→" Unicode: u2192 Rightwards Arrow |
| LeftRightArrow | `20` | "↔" Unicode: u2194 Left Right Arrow |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 Leftwards Double Arrow |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 Rightwards Double Arrow |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 Left Right Double Arrow |

### Examples

```csharp
// Called: node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
public void Equations_Type_EquationCombiningCharacterType()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    GroupCharacterEquationNode node = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
    node.Position = EquationCharacterPositionType.Top;
    node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

    EquationNode subBase = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
    TR.Text = "abc";

    string resultFile = Constants.destPath + "GroupCharacterEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);
    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    GroupCharacterEquationNode node2 = (GroupCharacterEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationNodeType.GroupChr, node2.EquationType);
    Assert.AreEqual(EquationCharacterPositionType.Top, node2.Position);
    Assert.AreEqual(EquationCombiningCharacterType.RightwardsDoubleArrow, node2.ChrType);
    Assert.AreEqual("⇒", node2.GroupChr);

    EquationNode node3 = node2.GetChild(0);
    Assert.AreNotEqual(null, node3);
    Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

    TR = (TextRunEquationNode)node3.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual("abc", TR.Text);
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


