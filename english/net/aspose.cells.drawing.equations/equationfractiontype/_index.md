---
title: Enum EquationFractionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationFractionType enum. This specifies the display style of the fraction bar
type: docs
url: /net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

This specifies the display style of the fraction bar.

```csharp
public enum EquationFractionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Bar | `0` | This specifies that the numerator is above and the denominator below is separated by a bar in the middle. |
| NoBar | `1` | This specifies that the numerator is above and the denominator below is not separated by a bar in the middle. |
| Linear | `2` | This specifies that the numerator is on the left and the denominator is on the right, separated by a '/' in between. |
| Skewed | `3` | This specifies that the numerator is on the upper left and the denominator is on the lower right, separated by a "/". |

### Examples

```csharp
// Called: Assert.AreEqual(EquationFractionType.Skewed, node2.FractionType);
public void Equations_Type_EquationFractionType()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    //test insert Fraction
    FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
    node.FractionType = EquationFractionType.Skewed;

    string str1 = "A";
    EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
    TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
    TR.Text = str1;

    string str2 = "B";
    EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
    TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
    TR.Text = str2;

    workbook.Save(Constants.destPath + "FractionEquationTest.xlsx");
    workbook = new Workbook(Constants.destPath + "FractionEquationTest.xlsx");

    TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    FractionEquationNode node2 = (FractionEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationFractionType.Skewed, node2.FractionType);

    EquationComponentNode numerator2 = (EquationComponentNode)node2.GetChild(0);
    Assert.AreNotEqual(null, numerator2);
    Assert.AreEqual(EquationNodeType.Numerator, numerator2.EquationType);

    EquationComponentNode denominator2 = (EquationComponentNode)node2.GetChild(1);
    Assert.AreNotEqual(null, denominator2);
    Assert.AreEqual(EquationNodeType.Denominator, denominator2.EquationType);

    TextRunEquationNode TR1 = (TextRunEquationNode)numerator2.GetChild(0);
    Assert.AreNotEqual(null, TR1);
    Assert.AreEqual(str1, TR1.Text);

    TextRunEquationNode TR2 = (TextRunEquationNode)denominator2.GetChild(0);
    Assert.AreNotEqual(null, TR2);
    Assert.AreEqual(str2, TR2.Text);

}
```

### See Also

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


