---
title: Enum EquationCharacterPositionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationCharacterPositionType enum. Specifies the position of a particular subobject within its parent
type: docs
url: /net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

Specifies the position of a particular subobject within its parent

```csharp
public enum EquationCharacterPositionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Top | `0` | At the top of the parent object |
| Bottom | `1` | At the bottom of the parent object |

### Examples

```csharp
// Called: Assert.AreEqual(EquationCharacterPositionType.Top, node2.BarPosition);
public void Equations_Type_EquationCharacterPositionType()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    BarEquationNode node = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
    node.BarPosition = EquationCharacterPositionType.Top;

    EquationNode subBase = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
    TR.Text = "x";

    string resultFile = Constants.destPath + "BarEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);

    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    BarEquationNode node2 = (BarEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationNodeType.Bar, node2.EquationType);
    Assert.AreEqual(EquationCharacterPositionType.Top, node2.BarPosition);

    EquationNode node3 = node2.GetChild(0);
    Assert.AreNotEqual(null, node3);
    Assert.AreEqual(EquationNodeType.Base, node3.EquationType);

    TR = (TextRunEquationNode)node3.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual("x", TR.Text);
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


